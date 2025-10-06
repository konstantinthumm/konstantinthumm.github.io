---
layout: single
title: "Konstantin Thumm"
subtitle: "Digitale Transformation, Projektmanagement & KI in der Sozialwirtschaft"
author_profile: true
classes: ["wide","hero-tall","home-hero"] # optional

header:
  overlay_color: "#000"   # bleibt Dark-Skin-freundlich
  overlay_filter: 0.35
  overlay_image: /assets/images/posts/spidey-1600.jpg
  actions:
    - label: "Über mich"
      url: /about/
    - label: "Newsletter abonnieren"
      url: /newsletter/
excerpt: "Beratung & Klarheit für NGOs, Sozialunternehmen & öffentliche Hand."
---

## Was ich mache

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur pharetra, risus et tincidunt posuere, enim nisi dictum nunc, vitae ultrices arcu nunc nec lectus.

![Platzhalter Inline](/assets/images/posts/spidey-600.jpg){: .align-right width="240" }
Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Aenean lacinia bibendum nulla sed consectetur. Maecenas faucibus mollis interdum. Donec id elit non mi porta gravida at eget metus. Sed posuere consectetur est at lobortis.

<div style="clear: both;"></div>

Phasellus sed posuere nulla. Nulla vitae elit libero, a pharetra augue. Vestibulum id ligula porta felis euismod semper. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.

<div class="notice--primary about-block">
  <h2>Über mich</h2>
  <p>Ich begleite Organisationen mit 15+ Jahren Erfahrung an der Schnittstelle aus Strategie, Prozessen und Technologie.</p>
  <p><a class="btn btn--primary" href="/about/">Mehr erfahren</a></p>
</div>

## Neu im Blog
<p>Die neuesten Beiträge findest du gebündelt auf der <a href="/posts/">Posts-Übersicht</a>.</p>
<div class="posts--home-grid">
  {% assign recent = site.posts | where_exp: "p", "p.hidden != true" %}
  {% for post in recent limit:3 %}
    <article class="archive__item">
      <a class="archive__item-teaser" href="{{ post.url | relative_url }}">
        <img src="{{ post.teaser | default: site.teaser }}" alt="{{ post.title | escape }}">
      </a>
      <h3 class="archive__item-title" style="margin-top:.5rem;">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p class="archive__item-excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>
    </article>
  {% endfor %}
</div>



## Newsletter
<p>Kurz, fokussiert, unregelmäßig — direkt aus Projekten & Recherchen.</p>
<!-- Buttondown/Newsletter-Einbettung oder Link -->
<p><a class="btn btn--primary" href="/newsletter/">Zur Anmeldung</a></p>

## Kontakt
<p>Kooperation anfragen? <a class="btn" href="/contact/">Hier entlang</a></p>
