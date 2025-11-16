---
layout: single
title: "Digitale Strukturen und Change Management"
description: "Wie Informationsarchitektur, Mandantenfähigkeit und Change-Management zusammenwirken – Grundlagen, Prinzipien und Projektbezug aus föderalen Organisationen."
permalink: /glossar/digitale-struktur-und-change/
toc: true
toc_sticky: true
toc_label: "Auf dieser Seite"
seo:
  title: "Digitale Strukturen und Change-Management – Architektur, Mandantenfähigkeit & Wandel"
  description: "Wie digitale Architektur, Mandantenfähigkeit und Change-Management Organisationen verändern – mit Beispielen aus föderalen Projekten."
  type: article
  image: /assets/images/og/konstantinthumm-de-1200.webp

---

Diese Seite bündelt zentrale Begriffe, die an der Schnittstelle von **digitaler Architektur**, **Organisation** und **Veränderung** liegen.
Sie zeigen, dass Technologie nie neutral ist – sie prägt, wie Menschen arbeiten, entscheiden und sich organisieren.

---

## Informationsarchitektur
{: #informationsarchitektur }

**Informationsarchitektur (IA)** beschreibt, wie Inhalte und Navigation in digitalen Systemen strukturiert sind, damit Menschen **finden, verstehen und handeln** können.
Gute IA schafft Klarheit, reduziert kognitive Last und lenkt Aufmerksamkeit. Sie ist der unsichtbare Rahmen, der aus Informationsfülle Orientierung macht.

In komplexen Organisationen – etwa in föderalen Verbänden oder großen NGOs – entscheidet die Informationsarchitektur darüber, ob eine Plattform verstanden oder als Hürde erlebt wird.
Eine klare IA gliedert Inhalte, trennt Zuständigkeiten und definiert eine konsistente **URL-Logik**.

**Kernelemente:**
- Inhaltsmodelle (z. B. News, Projekte, Services, Jobs)
- Navigationsstruktur (Hierarchie, Querverweise, Kontextlinks)
- Taxonomien (Kategorien, Tags, Metadaten)
- Visuelle Signale (Menüs, Breadcrumbs, Teaserlogik)

**Im Projektbezug:**
Beim *Webrelaunch eines Sozialverbands* entstand eine gemeinsame Struktur für Bundes- und Landesebene.
Die IA wurde damit zum **Organisationsmodell in digitaler Form**: Sie zeigte, wo Verantwortung beginnt und wo sie endet.

---

## Mandantenfähigkeit
{: #mandantenfaehigkeit }

**Mandantenfähigkeit** bedeutet, mehrere organisatorische Einheiten innerhalb einer technischen Plattform zu betreiben – **gemeinsame Basis, getrennte Datenräume**.
Es ist das digitale Äquivalent zu föderalen Systemen: jede Einheit (Mandant) besitzt Autonomie, bleibt aber in eine gemeinsame Infrastruktur eingebettet.

**Prinzipien:**
- Trennung von Daten und Konfiguration je Mandant
- Gemeinsamer Code- und Komponenten-Pool
- Zentrale Sicherheits-, Update- und Performance-Kontrolle
- Einheitliche Corporate-Design-Vorgaben
- Optional gemeinsame Datenquellen (z. B. Stellen-Datenbank)

**Bezug zum Sozialverbands-Projekt:**
Die Master-Clone-Architektur ist eine **praktische Umsetzung von Mandantenfähigkeit**.
Bund und Länder teilen eine Plattform – der Bund betreibt die Master-Instanz, die Länder nutzen Klone mit eigener Navigation und Inhalten.
So entsteht Einheitlichkeit ohne Zentralismus.

---

## Change-Management
{: #change-management }

**Change-Management** beschreibt den bewussten Prozess, Menschen, Strukturen und Technologien in Einklang zu bringen, wenn Wandel unvermeidlich oder gewollt ist.
Es verbindet Strategie, Kommunikation und Kultur.

**Ziele:**
- Veränderung **verstehbar** machen (Sinnvermittlung)
- Beteiligung **ermöglichen** (Dialogformate, Workshops)
- Kompetenzen **aufbauen** (Training, Guidelines)
- Ergebnisse **stabilisieren** (Routinen, Erfolgsmessung)

**Phasenmodell (verkürzt):**
1. **Erkennen** – Warum ist Veränderung nötig?
2. **Verstehen** – Welche Wirkung hat sie auf wen?
3. **Gestalten** – Wie kann sie konkret umgesetzt werden?
4. **Verankern** – Wie wird sie zum Alltag?

**Im Projektbezug:**
Beim Relaunch des Sozialverbands war Change kein Nebenprodukt, sondern zentrales Ziel.
Erst als Vertrauen und Sinn klar waren („Einheit durch Autonomie“), konnte Technik überhaupt akzeptiert werden.
Change-Management wurde so zur **unsichtbaren Infrastruktur** des Erfolgs.

---

## Projektbezug

{% assign term = site.data.glossar | where: "slug", "change-management" | first %}
{% if term and term.projects %}
  {% assign proj_ids = term.projects %}
  <div class="glossar-grid">
    {% for pid in proj_ids %}
      {% assign p = site.data.projects | where: "id", pid | first %}
      {% if p %}
        {% assign teaser = p.hero.teaser | default: p.hero.image %}
        <article class="glossar-card">
          <a href="{{ p.url }}">
            <img src="{{ teaser }}" alt="{{ p.title }}" loading="lazy" class="card-thumb">
          </a>
          <h3><a href="{{ p.url }}">{{ p.title }}</a></h3>
          {% if p.seo and p.seo.description %}<p>{{ p.seo.description }}</p>{% endif %}
          <a href="{{ p.url }}" class="btn btn--primary">Zum Projekt</a>
        </article>
      {% endif %}
    {% endfor %}
  </div>
{% endif %}

