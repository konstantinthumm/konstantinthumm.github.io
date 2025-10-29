---
layout: single
classes: ["wide","hero-tall","project-page"]
title: "Souveräne Infrastruktur für viele – Teil 2: Open-Source-Plattform fürs Ehrenamt"
excerpt: "Digitale Identität, Open-Source-Lösungen und echte Teilhabe: Wie ein Verband die Idee einer föderalen IT-Architektur weiterdachte – von M365 im Hauptamt zur offenen Plattform für das Ehrenamt."
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
  title: "Open-Source-Lösungen für das Ehrenamt – IT-Architekturkonzept (Teil 2)"
  description: "OpenXchange, Rocket.Chat, OpenTalk: Wie eine SSO-basierte Ehrenamtsplattform Identität, Datenschutz und Zusammenarbeit vereint – als kosteneffiziente Ergänzung zu M365 im Hauptamt."
  image: /assets/images/projects/it-architektur-teil2-1200.webp
  og_type: article
tags: [strategie, infrastruktur, change, sozialwirtschaft, opensource, collaboration, digitalisierung]
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

> „Wenn Zugehörigkeit digital wird, entsteht Teilhabe auf einer neuen Ebene.
> Nicht Technik steht im Mittelpunkt, sondern das Gefühl, verbunden zu sein – sichtbar, ansprechbar, beteiligt.“

## Ausgangspunkt – Zugehörigkeit sichtbar machen

Am Anfang stand eine simple, aber tiefgreifende Frage:
Wie kann man das, was tausende Menschen im Ehrenamt leisten, auch **digital sichtbar machen**?
Denn Engagement war überall – in Ortsgruppen, Projekten, Initiativen – doch technisch blieb vieles unsichtbar.
Jede*r nutzte eigene Mailkonten, Cloudspeicher oder Messenger. Kommunikation verlief quer, manchmal gar nicht.

Im Kern ging es also nicht um Tools, sondern um **Zugehörigkeit**:
Wie lässt sich spürbar machen, dass alle Teil derselben Organisation sind – auch digital?

> „Identität ist das, was bleibt, wenn alles Technische abstrahiert ist: das Gefühl, dazuzugehören.“


## Konzept – Identität als Fundament, nicht als Nachtrag

Die Lösung begann nicht bei der Software, sondern bei einem Prinzip: **Identität zuerst**.
Denn ohne digitale Identität bleibt jede Plattform ein Tor ohne Schlüssel.
Das Ziel war, alle Engagierten über eine **einheitliche Mailadresse auf Basis von [Open-Xchange (OX)](../glossar/it-architektur/#openxchange)** in das System zu integrieren –
als sichtbarer Ausdruck, dass sie dazugehören.

Damit verbunden: ein zentrales **Identitätsmanagement** (IDM) und **[Single Sign-On (SSO)](../glossar/it-architektur/#sso)**,
um später weitere Dienste wie **[OpenTalk](../glossar/it-architektur/#opentalk)**, **[Rocket.Chat](../glossar/it-architektur/#rocket-chat)** oder andere Systeme anzubinden.
Technik wurde hier nicht zum Selbstzweck, sondern zum Vehikel, um Verbundenheit zu schaffen –
zwischen Haupt- und Ehrenamt, zwischen Struktur und Mensch.


## Der Open-Source-Baukasten – offen, souverän, skalierbar

Das Fundament bildete eine Plattform aus bewährten, europäischen Open-Source-Komponenten:

- **Open-Xchange** für Mail, Kalender, Kontakte und Drive
- **Rocket.Chat** für die tägliche Zusammenarbeit in Gruppen und Kanälen
- **OpenTalk** für Videokonferenzen – stabil, datenschutzkonform und ohne Abhängigkeit von US-Anbietern

Alles verbunden über ein gemeinsames Login mit **SSO** – ein Zugang, viele Werkzeuge.
So entstand eine Architektur, die nicht zentralisiert, sondern vereint.
Ein System, das Datenschutz, Autonomie und Gemeinschaft gleichermaßen ernst nimmt.

> *Open Source war hier keine Ideologie, sondern eine Haltung:
> Kontrolle über Daten, Fairness gegenüber Ehrenamtlichen und Vertrauen in offene Standards.*


## So sah das Konzept konkret aus – praxisnah und verständlich

Das Konzept sah vor, dass möglichst alle ehrenamtlich Engagierten eine **Mailadresse über Open-Xchange** erhalten.
Damit würden sie in die neue Architektur eingebunden – nicht als technische Nutzer, sondern als Teil der Gemeinschaft.
Über diese Plattform könnten sie E-Mails schreiben, den Kalender pflegen und über regionale Adressbücher
die jeweils relevanten Personengruppen suchen, erreichen und anschreiben.

Das dazugehörige **Drive** – der Cloudspeicher mit Online-Office –
würde für Textverarbeitung, Tabellenkalkulation, Listen und Planungen genutzt werden.
Damit entstünde eine gemeinsame, barrierefreie Arbeitsumgebung – unabhängig von Gerät, Ort oder technischer Vorerfahrung.

Dieser erste Schritt war entscheidend:
Alle ins Identitätsmanagement zu bringen, um anschließend über **SSO** neue Dienste anbinden zu können.
Das **OpenID-Verzeichnis** fungiert dabei als zentrale Basis,
die jedem Konto eine Rolle, eine Gruppe und eine Zugehörigkeit zuordnet.
Darauf lassen sich Strukturen des Verbands – Land, Kreis, Bezirk, Ort – abbilden.
So entsteht ein Kommunikationsnetz, das formale Ebenen in echte Verbindung übersetzt.

> „Technik kann Nähe schaffen, wenn sie versteht, wie Menschen miteinander arbeiten wollen.“

In großen Verbänden droht oft Entfremdung:
Ortsgruppen fühlen sich abgehängt, während die Landesebene den Kontakt zur Basis verliert.
Genau hier lag die Stärke des Konzepts: durchdachte Kommunikationswege entlang realer Organisationslinien.
Information wird nicht mehr nach unten „verteilt“, sondern bewegt sich in beide Richtungen –
sichtbar, verbindlich, strukturiert.


## Perspektive – Brücken zwischen Haupt- und Ehrenamt

Das Konzept war von Anfang an so gedacht, dass es wachsen kann.
Sobald die Ehrenamtlichen über ihre Open-Xchange-Konten integriert sind,
lassen sich die Systeme von Haupt- und Ehrenamt technisch und organisatorisch verbinden:

- **Hybrid-ID** – die Föderation zwischen OpenID (Ehrenamt) und Entra ID (Hauptamt).
  Eine Identität, zwei Welten – verbunden über Vertrauen, aber mit getrennten Sicherheitsregeln.
- **SCIM / LDAP-Sync** – der automatische Abgleich von Gruppen, Rollen und Attributen.
  Statt mehrere Listen zu pflegen, werden Daten einmal gepflegt und überall aktuell.
- **Kalender-Feeds** über CalDAV und Graph-API – damit Termine ausgetauscht und sichtbar bleiben.
- **Kommunikations-Brücken** zwischen Rocket.Chat und Teams – damit Informationen fließen, nicht stocken.
- **Zentrales Adressbuch** über beide Systeme hinweg –
  nicht nur mit Namen, sondern mit Rollen und Verantwortlichkeiten, damit Zusammenarbeit auffindbar bleibt.

> Ein OpenID-Verzeichnis ist im Grunde eine Art digitales Adressbuch.
> Dort steht, wer dazugehört, welche Rolle er hat und auf welche Dienste er zugreifen darf.
> SSO bedeutet: einmal einloggen, alles nutzen.
> SCIM und LDAP sorgen dafür, dass diese Daten zwischen den Systemen synchron bleiben –
> so wie zwei Kalender, die sich gegenseitig aktualisieren.


## Entstehung – gewachsen aus Nähe, getragen von Vertrauen

Das Konzept entstand aus der täglichen Erfahrung in der Organisation.
Es wuchs aus Gesprächen mit Ehrenamtlichen, Landesgeschäftsstellen, IT-Partnern und Datenschutzbeauftragten.
Nichts war theoretisch – alles kam aus der Praxis.
Was anfangs nach Technik klang, wurde zu einem Symbol für Kulturwandel:
Nicht die IT sollte das Ehrenamt „digitalisieren“, sondern es **befähigen**.

Ein Beispiel blieb mir besonders im Kopf:
Ein kleiner Ortsverband, der bislang mit privaten Mailadressen arbeitete,
bekam seine ersten offiziellen Konten.
Plötzlich lief Kommunikation gebündelt, Termine waren abgestimmt,
und zum ersten Mal hieß es: *„Wir sind jetzt auch Teil der Plattform.“*
Das war kein IT-Erfolg – es war ein Organisationsmoment.


## Wirkung – Teilhabe in digitaler Form

Mit einer hohen fünfstelligen Zahl potenzieller Accounts wurde das Projekt
zu einem Beispiel für digitale Teilhabe im besten Sinn.
Identität wurde zur Eintrittskarte, Adressbücher zu Landkarten von Zuständigkeit,
und Single Sign-On zur Einladung, mitzumachen statt außen vor zu bleiben.

> „Digitalisierung gelingt nicht, wenn man sie verordnet.
> Sie gelingt, wenn Menschen sich eingeladen fühlen, Teil davon zu sein.“

So veränderte das Projekt die Haltung im Verband:
IT wurde nicht länger als Fremdkörper erlebt, sondern als Infrastruktur für Zusammenarbeit –
leise, funktional, hilfreich.


## Synthese – zwei Welten, ein Prinzip

Open Source fürs Ehrenamt ist nicht der Gegenentwurf zu M365,
sondern die zweite Hälfte derselben Idee:
ein Verband, zwei Systeme, eine Identität.

Digitale Architektur ist hier kein Bauplan aus Technik,
sondern eine **Organisationsgeschichte in Codeform**.
Sie zeigt, dass digitale Souveränität kein Ziel, sondern eine Haltung ist –
ein Weg, Verantwortung für Daten, Menschen und Zusammenarbeit bewusst zu gestalten.

> „Am Ende bleibt nicht das System in Erinnerung, sondern das, was es ermöglicht hat:
> echte Verbindung zwischen Menschen.“

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
