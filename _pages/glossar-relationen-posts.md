---
title: Glossar-Relationen – Posts → Begriffe (intern)
permalink: /intern/glossar-relationen-posts/
layout: single
toc: false
classes: wide
author_profile: false
sitemap: false
robots: noindex,nofollow
search: false
---

> Rückwärtsübersicht: Für jeden Blogpost die verknüpften Glossarbegriffe.

<div class="glossar-table full-bleed">
  <table class="table table--striped">
    <thead>
      <tr>
        <th>Post</th>
        <th>URL</th>
        <th>Glossarbegriffe</th>
      </tr>
    </thead>
    <tbody>

    {%- comment -%}
    URL-Kanonisierung ohne "startswith":
    - site.url / site.baseurl entfernen
    - führenden "/" sicherstellen
    - trailing "/" entfernen (außer bei "/")
    {%- endcomment -%}

    {%- assign all_posts = '' | split: '' -%}

    {%- for t in site.data.glossar -%}
      {%- if t.posts -%}
        {%- for p in t.posts -%}
          {%- assign raw = p.url | default: p.path | default: '' | strip -%}
          {%- if raw != '' -%}
            {%- assign canon = raw
              | replace: site.url, ''
              | replace: site.baseurl, ''
              | strip -%}

            {%- assign first = canon | slice: 0, 1 -%}
            {%- if first != '/' -%}{%- assign canon = '/' | append: canon -%}{%- endif -%}

            {%- assign last = canon | slice: -1, 1 -%}
            {%- if canon != '/' and last == '/' -%}{%- assign canon = canon | replace_last: '/', '' -%}{%- endif -%}

            {%- assign all_posts = all_posts | push: canon -%}
          {%- endif -%}
        {%- endfor -%}
      {%- endif -%}
    {%- endfor -%}

    {%- assign uniq_posts = all_posts | uniq -%}

    {%- for post_url in uniq_posts -%}
      {%- assign terms_for_post = '' | split: '' -%}
      {%- assign title_for_post = '' -%}

      {%- for t in site.data.glossar -%}
        {%- if t.posts -%}
          {%- for p in t.posts -%}
            {%- assign raw2 = p.url | default: p.path | default: '' | strip -%}
            {%- if raw2 != '' -%}
              {%- assign canon2 = raw2
                | replace: site.url, ''
                | replace: site.baseurl, ''
                | strip -%}

              {%- assign first2 = canon2 | slice: 0, 1 -%}
              {%- if first2 != '/' -%}{%- assign canon2 = '/' | append: canon2 -%}{%- endif -%}

              {%- assign last2 = canon2 | slice: -1, 1 -%}
              {%- if canon2 != '/' and last2 == '/' -%}{%- assign canon2 = canon2 | replace_last: '/', '' -%}{%- endif -%}

              {%- if canon2 == post_url -%}
                {%- assign terms_for_post = terms_for_post | push: t -%}
                {%- if title_for_post == '' and p.title -%}{%- assign title_for_post = p.title -%}{%- endif -%}
              {%- endif -%}
            {%- endif -%}
          {%- endfor -%}
        {%- endif -%}
      {%- endfor -%}

      <tr>
        <td>{{ title_for_post | default: "—" }}</td>
        <td><a href="{{ post_url | relative_url }}">{{ post_url }}</a></td>
        <td>
          {%- if terms_for_post.size > 0 -%}
            <ul>
              {%- for term in terms_for_post -%}
                <li>
                  {%- if term.url -%}
                    <a href="{{ term.url | relative_url }}">{{ term.term }}</a>
                  {%- else -%}
                    {{ term.term }}
                  {%- endif -%}
                </li>
              {%- endfor -%}
            </ul>
          {%- else -%}—{%- endif -%}
        </td>
      </tr>
    {%- endfor -%}

    </tbody>
  </table>
</div>
