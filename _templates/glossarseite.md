---
layout: single
title: "[THEMA ERSETZEN]"
permalink: /glossar/[slug-der-seite]/
description: "[SEO-Text – 1–2 Sätze, was diese Themenseite abdeckt]"
toc: true
toc_label: "Auf dieser Seite"
toc_sticky: true
---

## Begriff A
{: #slug-a }
[Kurzdefinition (1–3 Absätze), ggf. Bullet-Liste. Synonyme im laufenden Text erwähnen.]

## Begriff B
{: #slug-b }
[Ditto.]

## Begriff C
{: #slug-c }
[Ditto.]

---

{% comment %}
Slugs ALLER Begriffe, die auf dieser Glossarseite erklärt werden.
Nur Slugs mit `posts:` in _data/glossar.yml erzeugen am Ende Karten.
{% endcomment %}
{% assign page_slugs = "slug-a,slug-b,slug-c" | split: ',' %}
{% include glossar-post-cards.html slugs=page_slugs %}
