---
title: Intern – Übersichten & Debug-Tools
permalink: /intern/
layout: single
toc: false
classes: wide
author_profile: false
sitemap: false
robots: noindex,nofollow
search: false
---

{%- assign term_count = site.data.glossar | size -%}

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
        {%- assign first = canon | slice: 0,1 -%}
        {%- if first != '/' -%}{%- assign canon = '/' | append: canon -%}{%- endif -%}
        {%- assign last = canon | slice: -1,1 -%}
        {%- if canon != '/' and last == '/' -%}{%- assign canon = canon | replace_last: '/', '' -%}{%- endif -%}
        {%- assign all_posts = all_posts | push: canon -%}
      {%- endif -%}
    {%- endfor -%}
  {%- endif -%}
{%- endfor -%}
{%- assign post_count = all_posts | uniq | size -%}

{%- assign all_proj = '' | split: '' -%}
{%- for t in site.data.glossar -%}
  {%- if t.projects -%}
    {%- for pid in t.projects -%}{%- assign all_proj = all_proj | push: pid -%}{%- endfor -%}
  {%- endif -%}
{%- endfor -%}
{%- assign project_count = all_proj | uniq | size -%}

<div class="intern-grid">

  <div class="intern-card">
    <a class="intern-card__link" href="{{ '/intern/glossar-daten/' | relative_url }}">
      <span class="intern-icon">🐘</span>
      <span class="intern-title">Glossar-Daten</span>
      <span class="intern-desc">Alle Begriffe mit IDs, URLs, verknüpften Posts & Projekten.</span>
      <span class="meta"><strong>{{ term_count }}</strong> Begriffe</span>
    </a>
  </div>

  <div class="intern-card">
    <a class="intern-card__link" href="{{ '/intern/glossar-relationen-posts/' | relative_url }}">
      <span class="intern-icon">🚀</span>
      <span class="intern-title">Posts → Glossarbegriffe</span>
      <span class="intern-desc">Für jeden Blogpost die verlinkten Glossarbegriffe.</span>
      <span class="meta"><strong>{{ post_count }}</strong> verknüpfte Posts</span>
    </a>
  </div>

  <div class="intern-card">
    <a class="intern-card__link" href="{{ '/intern/glossar-relationen-projekte/' | relative_url }}">
      <span class="intern-icon">🎯</span>
      <span class="intern-title">Projekte → Glossarbegriffe</span>
      <span class="intern-desc">Für jede Projektseite die verlinkten Glossarbegriffe.</span>
      <span class="meta"><strong>{{ project_count }}</strong> Projekte</span>
    </a>
  </div>
</div>

<style>
.page__content .intern-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:1rem 1.25rem;
  margin:.5rem 0 1.25rem;
}
.page__content .intern-card{
  border-radius:.75rem;
  background:var(--background-alt,rgba(255,255,255,.03));
  border:1px solid rgba(255,255,255,.08);
}
.page__content .intern-card__link{
  display:block;
  padding:1.1rem 1.25rem 1rem;
  text-decoration:none;
  color:inherit;
  transition:transform .15s ease, box-shadow .15s ease;
}
.page__content .intern-card__link:hover{
  transform:translateY(-2px);
  box-shadow:0 6px 18px rgba(0,0,0,.15);
}
.page__content .intern-icon{ font-size:1.6rem; display:block; margin-bottom:.4rem; }
.page__content .intern-title{ display:block; font-weight:700; font-size:1.1rem; margin:.1rem 0 .25rem; }
.page__content .intern-desc{ display:block; margin:0 0 .35rem; opacity:.9; }
.page__content .meta{ display:block; opacity:.75; font-size:.95em; }
</style>
