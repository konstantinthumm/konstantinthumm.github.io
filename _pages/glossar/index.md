---
layout: single
title: "Glossar"
permalink: /glossar/
description: "Begriffe, die ich im Blog nutze – kurz erklärt. Mit Links zu weiterführenden Seiten."
toc: false
classes: wide
---

<div class="glossar-nav">
  {% assign letters = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z" | split: "," %}
  {% for L in letters %}
    <a href="#{{ L }}" class="pill">{{ L }}</a>
  {% endfor %}
</div>

<div class="glossar-compact" markdown="0">
  {% assign items = site.data.glossar | sort_natural: "term" %}
  {% assign grouped = items | group_by_exp: "i", "i.term | slice: 0, 1 | upcase" %}

  {% for group in grouped %}
    <h2 id="{{ group.name }}" class="glossar-letter">{{ group.name }}</h2>
    <ul class="glossar-list">
      {% for it in group.items %}
        <li>
          <a class="glossar-term" href="{{ it.url | relative_url }}">{{ it.term }}</a>
          {% if it.summary %}
            <span class="glossar-summary"> – {{ it.summary }}</span>
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  {% endfor %}
</div>

> Tipp: Fehlt dir ein Begriff? Schreib mir gern: [kt@konstantinthumm.de](mailto:kt@konstantinthumm.de).
