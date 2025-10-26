---
layout: single
title: "Schätzen und Prognostizieren"
permalink: /glossar/schaetzen-prognostizieren/
description: "Scrum Poker, Story Points und Velocity – wie Teams Komplexität verstehen, realistisch planen und empirisch lernen."
toc: true
toc_sticky: true
toc_label: "Auf dieser Seite"
---

## Scrum Poker
{: #scrum-poker }

**Scrum Poker** – auch *Planning Poker* genannt – ist eine spielerische Methode, um Aufwände und Komplexität gemeinsam einzuschätzen.
Statt starrer Zeitangaben wird der Aufwand **relativ** bewertet – typischerweise mit der Fibonacci-Skala (1, 2, 3, 5, 8 …).

Jedes Teammitglied wählt verdeckt eine Zahl, alle decken gleichzeitig auf.
Unterschiede in der Wahrnehmung führen zur Diskussion – genau dort liegt der Wert:
Nicht das Ergebnis, sondern der **Austausch** verbessert Verständnis und gemeinsame Lernbasis.

Scrum Poker verhindert Dominanz, macht implizites Wissen sichtbar und fördert psychologische Sicherheit.
Im Unterschied zu klassischen Aufwandsschätzungen geht es nicht um Vorhersage, sondern um Erkenntnis.

## Story Points
{: #story-points }

**Story Points** sind die Maßeinheit agiler Schätzung.
Sie messen **relative Komplexität**, nicht Zeit.
Eine Aufgabe mit 8 Punkten ist ungefähr doppelt so aufwendig wie eine mit 4 Punkten – abhängig vom Team.

Das Besondere: Story Points sind **team-spezifisch**.
Sie spiegeln die Leistungsfähigkeit, Erfahrung und Technologie eines Teams wider.
Erst durch wiederholte Beobachtung entsteht eine empirische Grundlage – die **Velocity**.
So entsteht Prognosefähigkeit durch Erfahrung, nicht durch Planung.

In klassischem Projektmanagement wären Story Points eine qualitative Ergänzung zu Kostenschätzungen – ein Werkzeug, um Unsicherheit messbar zu machen.

## Velocity
{: #velocity }

Die **Velocity** beschreibt, wie viele Story Points ein Team im Durchschnitt pro Sprint tatsächlich abschließt.
Sie ist keine Zielvorgabe, sondern ein **Beobachtungswert** – das Tempo, mit dem ein Team nachhaltig liefern kann.

Eine stabile Velocity entsteht erst nach mehreren Sprints.
Sie hilft, Forecasts zu erstellen, ohne Druck aufzubauen.
Wenn ein Team im Mittel 30 Story Points pro Sprint schafft und das Product Goal 120 Punkte umfasst, ist eine grobe Tendenz sichtbar – aber keine Verpflichtung.

Empirische Planung ersetzt so die Illusion exakter Kontrolle.
Auch in KI- oder Datenprojekten kann dieses Prinzip genutzt werden, um Komplexität zu steuern, ohne Kreativität zu behindern.

---

{% assign page_slugs = "..." | split: ',' %}
{% include glossar-post-cards.html slugs=page_slugs %}
