---
layout: single
title: "Projekte"
permalink: /projekte/
toc: false
classes: ["wide"]
---

## Projekte

{% assign projects = site.data.projects %}
{% if projects and projects.size > 0 %}
<ul class="project-list">
  {% for p in projects %}
  <li class="project-item">
    <a class="thumb" href="{{ p.url }}">
      <img src="{{ p.hero.teaser | default: p.hero.image }}" alt="{{ p.title }}" loading="lazy">
    </a>
    <div class="project-meta">
      <h3><a href="{{ p.url }}">{{ p.title }}</a></h3>
      {% if p.seo and p.seo.description %}<p>{{ p.seo.description }}</p>{% endif %}
      {% if p.status or p.domain %}
      <p class="badges">
        {% if p.status %}<span class="badge">{{ p.status }}</span>{% endif %}
        {% if p.domain %}<span class="badge">{{ p.domain }}</span>{% endif %}
      </p>
      {% endif %}
    </div>
  </li>
  {% endfor %}
</ul>
{% else %}
<p>Noch keine Projekte erfasst.</p>
{% endif %}
