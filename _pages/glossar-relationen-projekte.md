---
title: Glossar-Relationen – Projekte → Begriffe (intern)
permalink: /intern/glossar-relationen-projekte/
layout: single
toc: false
classes: wide
author_profile: false
sitemap: false
robots: noindex,nofollow
search: false
---

> Rückwärtsübersicht: Für jede Projektseite die verknüpften Glossarbegriffe.

<div class="glossar-table full-bleed">
  <table class="table table--striped">
    <thead>
      <tr>
        <th>Projekt</th>
        <th>URL</th>
        <th>Glossarbegriffe</th>
      </tr>
    </thead>
    <tbody>

    {%- assign all_proj_ids = '' | split: '' -%}
    {%- for t in site.data.glossar -%}
      {%- if t.projects -%}
        {%- for pid in t.projects -%}
          {%- assign all_proj_ids = all_proj_ids | push: pid -%}
        {%- endfor -%}
      {%- endif -%}
    {%- endfor -%}
    {%- assign uniq_proj_ids = all_proj_ids | uniq -%}

    {%- for pid in uniq_proj_ids -%}
      {%- assign terms_for_proj = '' | split: '' -%}

      {%- for t in site.data.glossar -%}
        {%- if t.projects contains pid -%}
          {%- assign terms_for_proj = terms_for_proj | push: t -%}
        {%- endif -%}
      {%- endfor -%}

      {%- assign project_obj = site.data.projects | where: "id", pid | first -%}

      <tr>
        <td>{{ project_obj.title | default: pid }}</td>
        <td>
          {%- if project_obj.url -%}
            <a href="{{ project_obj.url | relative_url }}">{{ project_obj.url }}</a>
          {%- else -%}
            —
          {%- endif -%}
        </td>
        <td>
          {%- if terms_for_proj.size > 0 -%}
            <ul>
              {%- for term in terms_for_proj -%}
                <li>
                  {%- if term.url -%}
                    <a href="{{ term.url | relative_url }}">{{ term.term }}</a>
                  {%- else -%}
                    {{ term.term }}
                  {%- endif -%}
                </li>
              {%- endfor -%}
            </ul>
          {%- else -%}
            —
          {%- endif -%}
        </td>
      </tr>

    {%- endfor -%}

    </tbody>
  </table>
</div>
