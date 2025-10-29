---
layout: single
classes: ["wide","hero-tall","project-page"]
title: "Von föderaler Vielfalt zur gemeinsamen Cloud – Teil 1: M365 als Plattform für das Hauptamt"
excerpt: "Wie eine durchdachte Microsoft-365-Architektur die Brücke zwischen zentraler Verantwortung und föderaler Autonomie schlagen sollte – und was wir über Entscheidungsprozesse in Verbänden gelernt haben."
permalink: /projekte/it-architektur-verband-teil1/
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
  title: "M365 als Plattform für das Hauptamt – IT-Architekturkonzept (Teil 1)"
  description: "Strategie, Governance, Change: Wie eine Multi-Tenant-Architektur auf Microsoft 365 eine gemeinsame Arbeitsumgebung für einen großen Verband schaffen sollte – mit föderaler Autonomie über Exchange-Admin-Rollen."
  image: /assets/images/projects/it-architektur-teil1-1200.webp
  og_type: article
tags: [strategie, infrastruktur, change, sozialwirtschaft, microsoft365, cloud, digitalisierung]
glossar_ids:
  - g-ms365
  - g-zero-trust
  - g-identity-management
  - g-tenant
  - g-multitenant
  - g-sso
  - g-active-directory
  - g-exchange
  - g-collaboration
  - g-subdomain
  - g-domain
---

> „Gemeinsam arbeiten heißt nicht, Kontrolle abzugeben –
> sondern Vertrauen in Strukturen zu übersetzen, die Zusammenarbeit ermöglichen.“

## Ausgangslage – viele gute Gründe, ein gemeinsames Ziel

Die Geschichte beginnt nicht mit Servern oder Lizenzen, sondern mit einem Verband, der größer, vielfältiger und dezentraler kaum sein könnte.
Über Jahrzehnte hatten sich in 16 Landesverbänden und zahlreichen Untergliederungen eigenständige IT-Lösungen etabliert – jedes System gewachsen, jedes aus bestem Grund entstanden.
Doch diese Vielfalt hatte ihren Preis: Komplexität, Redundanz und ein schleichender Verlust gemeinsamer Standards.

Zwar existierte eine gemeinsame Mail-Domain, die eine gewisse formale Einheit vermittelte.
Doch dahinter arbeiteten alle in separaten, unverbundenen Welten – von Outlook über lokale NAS-Laufwerke bis hin zu teils privat genutzten Cloud-Speichern.
Informationen verliefen im Zickzack durch den Verband, und Zusammenarbeit war oft von individuellen Routinen abhängig statt von gemeinsamer Struktur.

Der Bundesverband, organisatorisch Dach und Impulsgeber, suchte deshalb nach einer Lösung, die nicht zentralisiert, sondern verbindet:
eine Plattform, die Kommunikation erleichtert, Zusammenarbeit ermöglicht und die Kultur der Eigenverantwortung respektiert.
Genau an diesem Punkt begann meine Aufgabe.

## Anforderungen – formulierte Wünsche und unausgesprochene Erwartungen

In den Gesprächen mit den Ländern zeigte sich ein wiederkehrendes Muster:
Niemand wollte Kontrolle abgeben, aber alle wollten besser zusammenarbeiten.

Die Anforderungen ließen sich grob in drei Kategorien bündeln:

1. Einheitliche Grundlage: gemeinsame Mail-Infrastruktur, zentrale Sicherheitsstandards, klar definierte Governance.
2. Regionale Verantwortung: die Möglichkeit, innerhalb dieser Leitplanken eigenständig zu handeln.
3. Zukunftsfähigkeit: eine Architektur, die den Spagat zwischen Compliance, Datenschutz und Benutzerfreundlichkeit schafft.

Diese Anforderungen waren nicht nur technisch, sondern zutiefst organisatorisch.
Sie spiegelten die föderale DNA des Verbandes wider – ein Zusammenspiel von Vertrauen, Zuständigkeit und gelebter Autonomie.
Aus dieser Spannung heraus entstand die Idee einer föderal gedachten Microsoft-365-Architektur:
eine Cloud, die alle verbindet, ohne jemanden zu bevormunden.

## Konzept – von der Vision zur Struktur

Das Zielbild basierte auf drei Prinzipien: Einheit, Sicherheit und Autonomie.
Kern war eine Multi-Tenant-Architektur, in der der Bundesverband den Rahmen vorgibt,
während die Länder eigene Subdomains und definierte Administrationsrechte erhalten.
Jeder Landesverband sollte so in der Lage sein, seine Organisation eigenständig zu verwalten –
mit eigenen Exchange-Admins, die in der föderalen Gesamtstruktur verankert sind.

Diese Architektur verband klare Governance mit technischer Flexibilität.
Azure AD (heute Entra ID) sollte als zentrales Identitäts-Backbone dienen; Zero-Trust-Prinzipien wurden von Anfang an mitgedacht.
Sicherheit war kein nachträglicher Anstrich, sondern integraler Bestandteil des Designs.

Am Ende stand ein Zielbild:
eine gemeinsame Arbeitsumgebung, die E-Mail, Kalender, Datenablage und Kollaboration in einem konsistenten Ökosystem bündelt.
Nicht als monolithische Lösung, sondern als orchestrierte Struktur, die Vielfalt zulässt, aber Chaos verhindert.

> „Föderale Systeme brauchen Rahmen, keine Fesseln.“

## Umsetzungshindernisse – zwischen Machbarkeit und Mentalität

Das Projekt war ambitioniert.
Auf dem Papier klar, in der Praxis herausfordernd.
Ein föderaler Verband ist kein Konzern – Entscheidungsprozesse folgen anderen Logiken.
Selbst gute Ideen müssen erst gemeinschaftsfähig werden.

Das bedeutete intensive Abstimmungen mit Datenschutzbeauftragten, Betriebsrat, IT-Abteilungen und Vorständen.
In Workshops und Planungssitzungen wurde die Balance zwischen Vertrauen und Kontrolle immer wieder neu verhandelt.
Fragen nach der Rolle des Bundesverbands, nach Datensouveränität und nach der Sichtbarkeit der Länder im System bestimmten die Diskussionen.

Parallel liefen technische Evaluationen mit einem erfahrenen Systemhaus, das die Multi-Tenant-Struktur konzipierte
und einen umfassenden Change-Prozess auf Basis des ProSci-Frameworks vorschlug.

Doch während sich die technische Roadmap konkretisierte, blieb der kulturelle Unterbau fragil.
Einzelne Stakeholder äußerten Bedenken, insbesondere im Hinblick auf Datenschutz und Cloud-Souveränität.
Am Ende führte ein Veto auf Vorstandsebene dazu, dass das Projekt in der Planungsphase beendet wurde –
ein Rückschlag, aber kein Scheitern.

> „Nicht jedes gute Konzept muss umgesetzt werden, um Wirkung zu entfalten.“

## Verbandsstrukturen – Entscheidungslogik als Teil des Systems

Wer in Verbänden Projekte dieser Größenordnung verantwortet, lernt schnell:
Erfolg misst sich nicht nur am Ergebnis, sondern an der Fähigkeit, Entscheidungsprozesse zu gestalten.
Ein Verband ist keine hierarchische Organisation mit klarer Befehlskette,
sondern ein lebendiges Netzwerk aus Interessengruppen, Zuständigkeiten und Rollen.

Entscheidungen entstehen nicht linear, sondern im Aushandlungsprozess.
Ich habe gelernt, dass Technik in solchen Strukturen nicht primär eine Frage der Infrastruktur, sondern der Kultur ist.
Entscheidungen werden weniger durch Argumente als durch Vertrauen und gemeinsame Zielbilder getragen.
Ein technisches Konzept kann noch so tragfähig sein –
ohne eine klar strukturierte Beteiligung, ohne das Mitnehmen der Menschen, bleibt es Theorie.

Darum war dieses Projekt trotz seines Abbruchs von unschätzbarem Wert.
Es zeigte, wie wichtig es ist, frühzeitig alle Ebenen einzubinden, Entscheidungsräume zu definieren
und Change-Management als strategische Disziplin zu verstehen – nicht als Anhängsel der IT.

## Wirkung – was bleibt, auch ohne Rollout

Die technische Umsetzung fand nie statt, aber das Denken hat sich verändert.
Der Verband weiß heute, wie ein gemeinsamer digitaler Raum aussehen kann,
welche Voraussetzungen nötig sind und welche Stolpersteine zu vermeiden sind.

Der Weg, den wir beschrieben haben, dient inzwischen als Orientierung für neue Vorhaben –
vom Webrelaunch bis hin zu Prozessdigitalisierungen und Datenprojekten.

Ich sehe dieses Projekt als Blaupause für den Umgang mit komplexen Veränderungsprozessen.
Es hat nicht das System geschaffen, das geplant war –
aber es hat die Denkweise verändert, die nötig ist, um solche Systeme in Zukunft zu schaffen.

> „Manchmal ist das Wertvollste eines Projekts nicht das Ergebnis,
> sondern der gemeinsame Weg dorthin.“

## Synthese – Organisation in Codeform

M365 war in diesem Projekt mehr als ein Werkzeug.
Es war der Versuch, föderale Strukturen digital abzubilden, Vertrauen in Governance zu übersetzen
und Eigenständigkeit in technischer Architektur zu ermöglichen.

Auch wenn der Weg nicht zu Ende gegangen wurde, hat er Spuren hinterlassen –
in Prozessen, in Haltungen, in der Art, wie über Digitalisierung im Verband gesprochen wird.

Technik kann Organisation sichtbar machen –
und Organisation kann Technik scheitern lassen, wenn sie nicht reif dafür ist.
Beides gehört zusammen.

> „Digitale Architektur ist Organisationsentwicklung in Codeform –
> und entfaltet manchmal gerade dann Wirkung, wenn sie (noch) nicht gebaut wird.“

In diesem Sinne ist das Projekt weniger eine IT-Geschichte als eine Einladung zum gemeinsamen Denken: erst Klarheit, dann Struktur, dann Werkzeuge. Wer diese Reihenfolge respektiert, schafft Entscheidungsfähigkeit – und Raum für den nächsten Schritt.


<div class="project-crosslink no-thumb">
  <div class="project-crosslink__content">
    <p class="project-crosslink__eyebrow">Weiterlesen</p>
    <h3 class="project-crosslink__title">
      <a href="/projekte/it-architektur-verband-teil2/">Souveräne Infrastruktur für viele – Teil&nbsp;2: Open-Source-Plattform fürs Ehrenamt</a>
    </h3>
    <p class="project-crosslink__meta">
      Identität, SSO und Open-Source: Wie das Ehrenamt in die Architektur integriert wird.
    </p>
    <a class="btn btn--primary project-crosslink__cta" href="/projekte/it-architektur-verband-teil2/">Zu Teil&nbsp;2&nbsp;→</a>
  </div>
</div>




## Begriffe und Themen aus diesem Projekt

{% assign proj_id = "proj-it-architektur-teil1" %}
{% assign related_terms = site.data.glossar | where_exp: "t","t.projects contains proj_id" %}

<div class="glossar-grid">
  {% for t in related_terms %}
    <article class="glossar-card">
      <h3><a href="{{ t.anchors.page }}{{ t.anchors.fragment }}">{{ t.term }}</a></h3>
      <p>{{ t.summary }}</p>
    </article>
  {% endfor %}
</div>
