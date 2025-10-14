---
layout: single
title: "Glossar"
permalink: /glossar/
description: "Begriffe, die ich im Blog nutze – kurz erklärt. Mit Links zu weiterführenden Seiten."
toc: true
toc_sticky: true
toc_label: "Inhalt"
toc_h_min: 2
toc_h_max: 3
---

<div class="glossar-nav">
  {% assign letters = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z" | split: "," %}
  {% for L in letters %}
    <a href="#{{ L }}" class="pill">{{ L }}</a>
  {% endfor %}
</div>

<div class="glossar-listing" markdown="1">

{% assign items = site.data.glossar | sort_natural: "term" %}
{% assign grouped = items | group_by_exp: "i", "i.term | slice: 0, 1 | upcase" %}

{% for group in grouped %}
## {{ group.name }}
{:#{{ group.name }} .no_toc}

{% for it in group.items %}
### [{{ it.term }}]({{ it.url | relative_url }})
{:#{{ it.slug }}}
<p class="glossar-summary">– {{ it.summary }}</p>
{% endfor %}

{% endfor %}

</div>

> Tipp: Fehlt dir ein Begriff? Schreib mir gern: [kt@konstantinthumm.de](mailto:kt@konstantinthumm.de).
