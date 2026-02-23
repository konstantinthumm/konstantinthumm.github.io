---
layout: single
classes: ["wide","hero-tall","project-page"]
title: "Souveräne Infrastruktur für viele – Teil 2: Open-Source-Plattform fürs Ehrenamt"
excerpt: "Identity First statt Tool-Wildwuchs: Wie Open Source, SSO und Rollenmodelle digitale Teilhabe im Ehrenamt ermöglichen – und föderale Strukturen skalierbar machen."
permalink: /projekte/it-architektur-verband-teil2/
author_profile: true
toc: true
toc_label: "Inhalt"
header:
  overlay_image: /assets/images/projects/it-architektur-2000.webp
  overlay_filter: 0.4
  overlay_color: "#091217"
  caption: >-
    Photo by <a href="https://unsplash.com/@chadpeltola?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Chad Peltola</a>
    <a href="https://unsplash.com/photos/gray-and-black-metal-bridge-near-forest-painting-PacWLzKKTso?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

seo:
  title: "Open-Source-Plattform fürs Ehrenamt – IT-Architekturkonzept (Teil 2)"
  description: "Open-Xchange, Rocket.Chat, OpenTalk: Wie eine SSO-basierte Ehrenamtsplattform Identität, Datenschutz und Zusammenarbeit vereint – als souveräne Ergänzung zur M365-Welt."
  image: /assets/images/projects/it-architektur-teil2-1200.webp
  og_type: article

tags: [digitale-architektur, identity-management, open-source, non-profit, plattform-design, change-management]
glossar_ids:
  - g-openxchange
  - g-rocket-chat
  - g-opentalk
  - g-sso
  - g-identity-management
  - g-opensource
  - g-domain
  - g-subdomain
  - g-ldap
---

> „Digitale Zugehörigkeit beginnt mit Identität – nicht mit Software.“

## Ausgangspunkt – Ehrenamt ohne digitale Struktur

Während im Hauptamt über Cloud-Architektur diskutiert wurde, blieb das Ehrenamt technisch fragmentiert: private Mailkonten, uneinheitliche Messenger, keine zentrale Identitätslogik.

Das Problem war nicht fehlende Tools. Es war fehlende digitale Zugehörigkeit.

## Architekturprinzip – Identity First

Das Konzept setzte an der Wurzel an: **digitale Identität als Fundament.**

Ziel war:
- einheitliche Mailidentität über Open-Xchange,
- zentrales Identitätsmanagement,
- Single Sign-On als verbindendes Zugangssystem,
- Rollen- und Gruppenzuordnung entlang realer Verbandsstrukturen.

Erst Identität. Dann Plattform.

## Plattform-Design – offene Architektur statt Tool-Sammlung

Die Lösung bestand aus einem modularen Open-Source-Stack:
- Open-Xchange (Mail, Kalender, Drive),
- Rocket.Chat (Zusammenarbeit),
- OpenTalk (Videokonferenz),
- SSO & LDAP/SCIM-Synchronisation.

Technik diente hier einem strukturellen Ziel: Zugehörigkeit sichtbar machen, Kommunikationswege entlang realer Organisationslinien abbilden und Autonomie sichern.

> „Open Source war hier keine Ideologie, sondern eine pragmatische Souveränitätsentscheidung.“

## Meine Rolle – Brücke zwischen Struktur und Umsetzung

Ich entwickelte das konzeptionelle Integrationsmodell:
- Identitäts- und Rollenmodell für föderale Ebenen (Land, Kreis, Ort),
- SSO- und Verzeichnislogik (Gruppen, Attribute, Zuständigkeiten),
- Synchronisations- und Skalierungsprinzipien für spätere Erweiterungen.

So wurde aus „Ehrenamt digitalisieren“ ein Strukturansatz: **Teilnahme über Identität, Zusammenarbeit über klare Wege.**

## Integrationsperspektive – Hauptamt und Ehrenamt verbinden, ohne zu vermischen

Das Konzept war so angelegt, dass es später anschlussfähig bleibt:
- Föderation zwischen OpenID (Ehrenamt) und Entra ID (Hauptamt),
- automatischer Abgleich von Gruppen/Rollen (SCIM/LDAP),
- Kalender- und Verzeichnis-Brücken,
- Kommunikationsbrücken zwischen Rocket.Chat und Teams.

Ziel: ein Verband, zwei Systemwelten – mit einer gemeinsamen Organisationslogik.

## Wirkung – Identität als Teilhabe

Mit potenziell fünfstelliger Nutzerzahl wurde Identität zur Eintrittskarte: Engagierte wurden systemisch sichtbar, Kommunikation wurde strukturell verankert, Plattform wurde als Infrastruktur verstanden – nicht als Fremdkörper.

> „Digitalisierung gelingt nicht, wenn man sie verordnet. Sie gelingt, wenn Menschen sich eingeladen fühlen.“

## Synthese – Zwei Systeme, ein Prinzip

Open Source fürs Ehrenamt ist kein Gegenentwurf zu M365, sondern die zweite Hälfte derselben Idee: föderale Strukturen digital abbilden, Verantwortung klar verorten, Teilhabe ermöglichen.

> „Plattformdesign ist Organisationsdesign.“

Das Ehrenamt sichtbar zu machen heißt, Identität ernst zu nehmen. Wenn Zugehörigkeit spürbar wird, folgen Zusammenarbeit und Verantwortung fast von selbst – und die Plattform wächst dort, wo sie gebraucht wird.

<div class="project-crosslink no-thumb">
  <div class="project-crosslink__content">
    <p class="project-crosslink__eyebrow">Weiterlesen</p>
    <h3 class="project-crosslink__title">
      <a href="/projekte/it-architektur-verband-teil1/">Von föderaler Vielfalt zur gemeinsamen Cloud – Teil&nbsp;1: M365 als Plattform für das Hauptamt</a>
    </h3>
    <p class="project-crosslink__meta">Governance, Multi-Tenant und föderale Verantwortlichkeiten als Fundament.</p>
    <a class="btn btn--primary project-crosslink__cta" href="/projekte/it-architektur-verband-teil1/">Zu Teil&nbsp;1&nbsp;→</a>
  </div>
</div>

## Begriffe und Themen aus diesem Projekt

{% assign proj_id = "proj-it-architektur-teil2" %}
{% assign related_terms = site.data.glossar | where_exp: "t","t.projects contains proj_id" %}

<div class="glossar-grid">
  {% for t in related_terms %}
    <article class="glossar-card">
      <h3><a href="{{ t.anchors.page }}{{ t.anchors.fragment }}">{{ t.term }}</a></h3>
      <p>{{ t.summary }}</p>
    </article>
  {% endfor %}
</div>