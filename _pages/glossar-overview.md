---
title: Glossar-Datenübersicht (intern)
permalink: /intern/glossar-daten/
layout: single
toc: false
classes: wide
author_profile: false

# Sichtbarkeit / SEO
sitemap: false
robots: noindex,nofollow
search: false

# Keine Navi-Verlinkung
sidebar:
  nav: ""
---

> Interne Prüfliste für alle Glossarbegriffe (IDs, URLs, verknüpfte Posts & Projekte).

<div class="glossar-table full-bleed">
  <table class="table table--striped">
    <thead>
        <tr>
        <th>Term</th>
        <th>Slug</th>
        <th>ID</th>
        <th>URL</th>
        <th>Posts</th>
        <th>Projects</th>
        </tr>
    </thead>
    <tbody>
    {% for t in site.data.glossar %}
        <tr>
        <td>{{ t.term }}</td>
        <td>{{ t.slug }}</td>
        <td><code>{{ t.id }}</code></td>
        <td>
            {% if t.url %}
            <a href="{{ t.url | relative_url }}">{{ t.url }}</a>
            {% elsif t.anchors %}
            {{ t.anchors.page }}#{{ t.anchors.fragment | remove: '#' }}
            {% endif %}
        </td>
        <td>
            {% if t.posts and t.posts.size > 0 %}
            <ul>
            {% for p in t.posts %}
                {% assign p_url = p.url | default: p.path %}
                <li>
                {% if p_url %}
                    <a href="{{ p_url | relative_url }}">{{ p.title | default: p_url }}</a>
                {% else %}
                    {{ p.title | default: '—' }}
                {% endif %}
                </li>
            {% endfor %}
            </ul>
            {% else %}
            —
            {% endif %}
        </td>
        <td>
            {% if t.projects and t.projects.size > 0 %}
            <code>{{ t.projects | join: ", " }}</code>
            {% else %}
            —
            {% endif %}
        </td>
        </tr>
    {% endfor %}
    </tbody>
</table>
</div>