---
layout: single
title: "Konstantin Thumm"
subtitle: "Digitale Transformation, Projektmanagement & KI in der Sozialwirtschaft"
author_profile: true
classes: ["wide","hero-tall","home-hero","hero-wide"]

header:
  overlay_color: "#252a34"   # bleibt Dark-Skin-freundlich
  overlay_filter: 0.1
  overlay_image: /assets/images/hero/konstantinthumm-hero2.webp
  # actions:
  #  - label: "Über mich"
  #    url: /about/
  #  - label: "Newsletter abonnieren"
  #    url: /newsletter/
excerpt: "Wie verändert Digitalisierung unsere Arbeit - und was braucht es, damit sie gelingt?<br>Ich teile hier Gedanken, Erfahrungen und Perspektiven aus dem, was ich in Projekten erlebt, gelernt und ausprobiert habe."
---

## Warum Digitalisierung für mich mehr ist als Technik

Seit den 1990ern faszinieren mich das Internet, digitale Werkzeuge und alles, was mit technologischem Wandel zu tun hat. Aus Neugier wurde Beruf, aus Beruf Leidenschaft. Ich habe über die Jahre viele Seiten der IT kennengelernt – von Projekten in Unternehmen bis hin zu Aufgaben, bei denen Menschen und Technologie aufeinandertreffen.

Heute beschäftige ich mich besonders mit Themen rund um Projektmanagement, Künstliche Intelligenz und agile Methoden. Mich interessiert, wie Organisationen diese Entwicklungen so nutzen können, dass sie echten Mehrwert schaffen – für ihre Arbeit, ihre Teams und die Menschen, die sie erreichen wollen.

Digitalisierung bedeutet für mich nicht schneller, sondern bewusster zu werden: Zusammenhänge zu verstehen, Prozesse einfacher zu machen und Neues mutig auszuprobieren. Dabei geht es weniger um Tools, sondern darum, wie wir miteinander arbeiten und lernen.<br>
[Mehr über mich erfahren →](/about/)

### Was es braucht, damit sie gelingt

Ich habe keine fertigen Antworten – aber viele Fragen, Gedanken und Erfahrungen, die ich hier teile. In meinem Blog schreibe ich über Grundlagen, Methoden und Beobachtungen aus der Praxis. Ich möchte Themen anstoßen, Denkanstöße geben und Diskussionen eröffnen.



## Neue Gedanken und Artikel im Blog
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
<hr>
Schauen Sie sich gern um, lesen Sie mit, diskutieren Sie mit mir im Blog oder auf [LinkedIn](https://www.linkedin.com/in/konstantinthumm), [Mastodon](https://social.tchncs.de/@konstantinthumm) oder [Bluesky](https://bsky.app/profile/konstantinthumm.bsky.social) – oder entdecken Sie einfach etwas, das Sie inspiriert.

<!-- Newsletter-Block vorübergehend deaktiviert.
     Hinweis: Später mit Mailtrain-Integration wieder einsetzen. -->
<!-- ## Newsletter
<p>Kurz, fokussiert, unregelmäßig — direkt aus Projekten & Recherchen.</p>
<p><a class="btn btn--primary" href="/newsletter/">Zur Anmeldung</a></p>
-->


