---
layout: single
title: "Konstantin Thumm"
subtitle: "Digitale Transformation, Projektmanagement & KI in der Sozialwirtschaft"
author_profile: true
classes: ["wide","hero-tall","home-hero","hero-wide","hero-focus-down"]

header:
  overlay_color: "#252a34"
  overlay_filter: 0.1
  overlay_image: /assets/images/hero/konstantinthumm-hero2.webp

excerpt: "Wie verändert Digitalisierung unsere Arbeit – und was braucht es, damit sie gelingt?<br>Ich teile hier Gedanken, Erfahrungen und Perspektiven aus dem,<br> was ich in Projekten erlebt, gelernt und ausprobiert habe."
---

## Worum es hier geht

Diese Website ist ein persönlicher Arbeits- und Denkraum.
Ich schreibe über digitale Transformation, Projektarbeit, Künstliche Intelligenz und Zusammenarbeit – nicht aus der Theorie, sondern aus Projekten, Beobachtungen und echter Praxis.

Mich interessiert weniger, welche Tools eingesetzt werden, sondern wie Organisationen Entscheidungen treffen, wie Prioritäten entstehen und was es braucht, damit Veränderung nicht nur geplant, sondern auch umgesetzt wird.

> Mehr zur Einordnung: In meinem Profil findest du eine kompakte Übersicht zu Rolle, Schwerpunkt und Kontext.
> → [Zum Profil](/profil/)

## Mein Blick auf Digitalisierung

Digitalisierung bedeutet für mich nicht, alles schneller zu machen.
Sie bedeutet, Komplexität zu reduzieren, Zusammenhänge besser zu verstehen und bewusst zu entscheiden, was wirklich hilft.

Oft geht es dabei weniger um Technik als um Fragen wie:
- Wer entscheidet eigentlich was?
- Wie entstehen Prioritäten?
- Wie arbeiten Menschen sinnvoll zusammen?

## Blog

Im Blog sammle ich Gedanken, Methoden und Beobachtungen aus der Praxis.
Mal geht es um Grundlagen, mal um konkrete Formate, mal um aktuelle Entwicklungen rund um KI und Organisationen.

> Einstiegshilfe: Wenn du nur stöbern willst, nimm die Blog-Übersicht. Wenn du wissen willst, wer hinter den Inhalten steht, nimm das Profil.
> → [Zur Blog-Übersicht](/posts/) · [Zum Profil](/profil/)

## Neue Gedanken und Artikel im Blog

<p>Die neuesten Beiträge findest du gebündelt in der <a href="/posts/">Blog-Übersicht</a>.</p>

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

Schau dich gern um, lies mit oder diskutiere mit mir im Blog oder auf
[LinkedIn](https://www.linkedin.com/in/konstantinthumm){:target="_blank" rel="noopener noreferrer" .ext},
[Mastodon](https://social.tchncs.de/@konstantinthumm){:target="_blank" rel="noopener noreferrer" .ext}
oder
[Bluesky](https://bsky.app/profile/konstantinthumm.bsky.social){:target="_blank" rel="noopener noreferrer" .ext}.


