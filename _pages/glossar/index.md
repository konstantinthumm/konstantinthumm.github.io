---
layout: single
title: "Glossar"
permalink: /glossar/
description: "Begriffe, die ich im Blog nutze – kurz erklärt. Mit Links zu weiterführenden Seiten."
toc: true
toc_sticky: true
toc_label: "Inhalt"
---

<div class="glossar-nav">
  {% assign letters = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z" | split: "," %}
  {% for L in letters %}
    <a href="#{{ L }}" class="pill">{{ L }}</a>
  {% endfor %}
</div>

{% assign items = site.data.glossar | sort_natural: "term" %}
{% assign grouped = items | group_by_exp: "i", "i.term | slice: 0, 1 | upcase" %}

{% for group in grouped %}
## {{ group.name }}
{: #{{ group.name }} }

<ul class="glossar-list">
  {% for it in group.items %}
  <li>
    <a href="{{ it.url | relative_url }}"><strong>{{ it.term }}</strong></a>
    <span class="glossar-summary">– {{ it.summary }}</span>
  </li>
  {% endfor %}
</ul>

{% endfor %}

> Tipp: Fehlt dir ein Begriff? Schreib mir gern: [kt@konstantinthumm.de](mailto:kt@konstantinthumm.de).
