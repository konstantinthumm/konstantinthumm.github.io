---
layout: single
classes: ["wide","hero-tall","project-page"]
title: "Wie föderale Vielfalt digitale Einheit schafft – der Webrelaunch eines Sozialverbands"
excerpt: "Ein föderaler Verband zwischen zentraler Identität und regionaler Autonomie: Wie eine durchdachte Webarchitektur den Stillstand überwand – und Einheit in Vielfalt ermöglichte."
permalink: /projekte/sozialverband-relaunch/
author_profile: true
toc: true
toc_label: "Inhalt"
header:
  overlay_image: /assets/images/projects/sozialverband-relaunch-hero-2000.webp
  overlay_filter: 0.4
  overlay_color: "#091217"
  caption: >-
    Master-Clone-Architektur für föderale Verbandsstrukturen<br>
    Photo by <a href="https://unsplash.com/@halacious?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Hal Gatewood</a> on
    <a href="https://unsplash.com/photos/assorted-color-comic-script-D-_zRKxP9Rw?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
seo:
  title: "Wie föderale Vielfalt digitale Einheit schafft – Webrelaunch eines Sozialverbands"
  description: "Von der komplexen TYPO3-Instanz zur modernen Master-Clone-Architektur: Ein föderaler Verband im digitalen Wandel – mit Stakeholder-Management, Change-Begleitung und Product Ownership."
  image: /assets/images/projects/sozialverband-relaunch-1200.webp
tags: [change, strategie, sozialwirtschaft]
glossar_ids:
  - g-stakeholder-management
  - g-autonomie
  - g-governance
  - g-informationsarchitektur
  - g-change-management
  - g-mandantenfaehigkeit
---

## Wie föderale Vielfalt digitale Einheit schafft – der Webrelaunch eines Sozialverbands

Über Jahre hinweg war die Website eines großen Sozialverbands gewachsen – ein lebendiges, aber zunehmend unübersichtliches Konstrukt aus Inhalten, Bildern, Extensions und Berechtigungen. Technisch basierte sie auf **TYPO3**, organisatorisch auf einem komplexen **Rollen- und Rechtekonzept** für Redakteur*innen aus Bund und Ländern. Jede regionale Instanz pflegte ihre Inhalte eigenständig, doch die gemeinsame Plattform hatte längst ihre Grenzen erreicht: veraltete Versionen, inkompatible Erweiterungen, Performanceprobleme – und vor allem: ein wachsender Konsensverlust zwischen den Beteiligten.

Denn wo viele Akteure gleichberechtigt gestalten wollen, droht leicht Stillstand. Der Bundesverband verstand sich als **Dach und Dienstleister** – verantwortlich für Außendarstellung, Struktur und Rahmenbedingungen. Die **Landesverbände** hingegen waren operativ tätig, nah an Mitgliedern und Themen. Während der Bund einheitliche Regeln und ein konsistentes Erscheinungsbild anstrebte, forderten die Länder mehr Autonomie und Gestaltungsspielraum. Zwischen föderaler Realität und zentraler Verantwortung entstand eine typische, aber hochkomplexe Verbandssituation: jeder mit guten Gründen, keiner mit Durchgriff.

Die **Arbeitsgruppe Website** sollte diese Interessen bündeln. Doch sie scheiterte an der eigenen demokratischen Perfektion. Sitzungen wurden zu Protokollorgien, Entscheidungen zerredet, und irgendwann blieb der Fortschritt auf der Strecke. Das Projekt drohte zu kollabieren – mit der radikalen Konsequenz, den gemeinsamen Webauftritt ganz aufzugeben.

## Product Ownership, Stakeholder-Management und Change-Prozess

An dieser Stelle begann mein Auftrag – und mein Beitrag.
Ich übernahm die Rolle des **Product Owners** und moderierte die Schnittstelle zwischen den **Stakeholdern auf Landesebene**, dem **Bundesverband** und der **externen Agentur**, die die technische Umsetzung verantwortete.
Diese Rolle war weniger formal als vielmehr **katalytisch**: Sie erforderte Empathie, Klarheit und das Vertrauen aller Beteiligten.

Zu Beginn stand nicht die Technik, sondern das Verständnis füreinander.
In einem intensiven **Stakeholder-Mapping** wurden die Interessen, Sorgen und Prioritäten der Länder sichtbar gemacht – von inhaltlicher Kontrolle über technische Abhängigkeiten bis hin zur Angst, „untergeordnet“ zu werden.
Ich moderierte diesen Prozess bewusst transparent: mit **Workshops, offenen Feedback-Runden** und einer großen **Informationsveranstaltung** für alle Landesgeschäftsführer*innen und Verantwortlichen der Öffentlichkeitsarbeit.

Hier ging es nicht um PowerPoint-Folien, sondern um Vertrauen.
Erst als klar war, dass das neue System **Freiheit nicht beschneidet, sondern strukturiert**, entstand die Bereitschaft zur Veränderung.
Das war **Change-Management** im eigentlichen Sinn:
Menschen emotional mitzunehmen, den Sinn hinter der Technik greifbar zu machen – und Widerstände als notwendige Signale zu verstehen.

## Technisches und organisatorisches Konzept

Ich schlug schließlich ein Konzept vor, das den scheinbaren Widerspruch zwischen Einheit und Autonomie auflöste: eine **Master-Clone-Architektur**.

Im Zentrum stand eine **Masterinstallation beim Bundesverband**.
Diese Instanz übernahm die Rolle des **technischen und organisatorischen Generalunternehmers** – mit klaren Standards und einer verlässlichen Infrastruktur:

- **Hosting, Design und Grundlayout:** zentral verwaltet und CI-konform
- **Backend und Programmierung:** standardisiert und zukunftssicher
- **Struktur und URL-Systematik:** einheitlich über alle Instanzen hinweg

Auf dieser Basis konnten die Länder **eigene Webseiten als Klone** der Masterinstallation aufbauen – unabhängig, aber nicht isoliert.
Sie erhielten damit die nötige **Freiheit in Inhalten und Navigation**, ohne die visuelle und technische Kohärenz der Gesamtorganisation zu gefährden.

Ein zentrales Element war die **gemeinsame Datenbank für Stellenangebote:**

- Auf den Landeswebseiten wurden nur regionale Ausschreibungen angezeigt.
- Auf der Bundeswebseite erschien automatisch eine **aggregierte Gesamtübersicht** aller Jobs im Verband.

So verband das System **dezentrale Pflege** mit **zentraler Sichtbarkeit** – eine elegante Lösung für ein altes Problem.

## Umsetzung & Technologie

Das Projekt wurde schließlich auf Basis einer **modernen Django/Python-Architektur** realisiert – als maßgeschneiderte Eigenentwicklung durch eine spezialisierte Agentur.
Als Product Owner verantwortete ich die **Backlog-Pflege, Priorisierung und Abstimmung** zwischen Verband und Agentur.
Ich übersetzte fachliche Anforderungen der Stakeholder in technische Spezifikationen und begleitete die iterative Umsetzung – ein agiler, pragmatischer Prozess, der durch klare Verantwortlichkeiten getragen wurde.

Alternativ wäre eine WordPress-Multisite-Variante denkbar gewesen, doch das Django-Konzept überzeugte durch **Stabilität, Performance und Flexibilität**.
Auch das **Design** spielte eine Schlüsselrolle: zeitgemäß, barrierearm, emotional ansprechend – und dennoch streng im Corporate Design verankert.

Die Lösung begeisterte schließlich alle Landesverbände.
Sie sahen, dass **technische Standardisierung nicht Verlust von Freiheit** bedeuten muss, sondern ihre Grundlage sein kann.
Die Kosten konnten aufgeteilt, Wartung und Sicherheit vereinheitlicht, Inhalte trotzdem individuell gestaltet werden.

## Synthese – Lehre aus dem Projekt

Dieses Projekt zeigt exemplarisch, dass **digitale Lösungen in Verbänden** nicht nur technische, sondern zutiefst **strukturelle und kulturelle Fragen** sind.
Wo föderale Organisationen zwischen Einheit und Vielfalt balancieren, kann Technologie ein moderierendes Prinzip sein – **nicht als Machtinstrument, sondern als Ermöglicher von Selbstbestimmung im Rahmen gemeinsamer Standards**.

Das **Stakeholder-Management** war dabei der Schlüssel: die Fähigkeit, Unterschiedlichkeit als Ressource zu verstehen und daraus eine gemeinsame digitale Sprache zu formen.
Und es zeigte, dass die Rolle des **Product Owners** weit über die technische Steuerung hinausgeht – sie ist **Brücke, Übersetzer und Gestalter von Veränderung**.

Das **Master-Clone-Konzept** bewies:
**Digitale Architektur ist Organisationsentwicklung in Codeform.**
Und wenn Technik richtig gedacht wird, kann sie genau das schaffen, was lange verhandelt wurde – **Einheit durch Autonomie**.


---

## Begriffe und Themen aus diesem Projekt

{% assign p = site.data.projects | where: "id", "proj-sozialverband-relaunch" | first %}
{% assign related_terms = site.data.glossar | where_exp: "t","t.projects contains p.id" %}

<div class="glossar-grid">
  {% for t in related_terms %}
    <article class="glossar-card">
      <h3><a href="{{ t.anchors.page }}{{ t.anchors.fragment }}">{{ t.term }}</a></h3>
      <p>{{ t.summary }}</p>
    </article>
  {% endfor %}
</div>


## Blogposts mit inhaltlichem Bezug

{% assign related_posts = site.data.glossar | map: "posts" | compact | flatten %}
{% assign filtered_posts = "" | split: "" %}
{% for term in site.data.glossar %}
  {% for post in term.posts %}
    {% if post.url == "/involvement-scrum-team/" %}
      {% assign filtered_posts = filtered_posts | push: post %}
    {% endif %}
  {% endfor %}
{% endfor %}

<div class="glossar-grid">
  {% for post in filtered_posts %}
    <article class="glossar-card">
      <a href="{{ post.url }}">
        <img src="{{ post.image }}" alt="{{ post.title }}" loading="lazy">
      </a>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}" class="btn btn--primary">{{ post.btn_label }}</a>
    </article>
  {% endfor %}
</div>

