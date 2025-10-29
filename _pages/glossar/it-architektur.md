---
layout: single
title: "IT-Architektur im Verband – Begriffe, die den Unterschied machen"
description: "Microsoft 365, Entra ID, Zero Trust, SSO und Domain-Management verständlich erklärt – Basis einer sicheren, föderalen IT-Architektur in Verbänden."
permalink: /glossar/it-architektur/
author_profile: true
toc: true
toc_sticky: true
toc_label: "Inhalt"
seo:
  title: "IT-Architektur im Verband – Microsoft 365, Zero Trust & Identitätsmanagement"
  description: "Zentrale Begriffe der IT-Architektur: Microsoft 365, Entra ID, Zero Trust, Identitäts- und Domain-Management als Basis föderaler Zusammenarbeit."
  type: article
  image: /assets/images/og/konstantinthumm-de-1200.webp

---

> Dieses Glossar bündelt zentrale Begriffe aus den Projekten „Von föderaler Vielfalt zur gemeinsamen Cloud – Teil 1“ und „Souveräne Infrastruktur für viele – Teil 2“. Ziel ist Verstehen mit Joy of Use: fundiert, praxisnah, ohne Marketingfloskeln.

## Microsoft 365 (M365)
{: #ms365 }

<a href="https://www.microsoft.com/microsoft-365" target="_blank" rel="noopener">Microsoft 365</a> ist mehr als ein Softwarepaket – es ist eine Infrastrukturphilosophie. Der Zusammenschluss aus Diensten wie [Exchange Online](#exchange), SharePoint, OneDrive und Teams bildet das Rückgrat einer modernen Arbeitsumgebung, die Kommunikation, Kollaboration und Identitätsmanagement vereint. Im Kern steht nicht die App-Liste, sondern das Zusammenspiel zwischen Benutzeridentitäten, Sicherheit, Richtlinien und Governance. In föderalen Organisationen ermöglicht M365, gemeinsame Standards zu etablieren, ohne lokale Freiheit aufzugeben – eine Balance aus Einheit und Autonomie.

Für große Verbände liegt die Stärke von M365 in seiner Fähigkeit, komplexe Strukturen abzubilden. Über Mandanten, [Subdomains](#subdomain) und differenzierte Admin-Rollen können einzelne Landesverbände eigenständig agieren, während der Bundesverband zentrale Leitplanken definiert. Governance-Modelle, [Zero Trust](#zero-trust)-Mechanismen und automatisiertes [Identitätsmanagement](#identity-management) schaffen dabei die Grundlage für Sicherheit und Transparenz. M365 ist damit kein Tool, sondern ein Organisationsrahmen, der Zusammenarbeit technisch und kulturell neu definiert.



## Zero Trust
{: #zero-trust }

Zero Trust ist ein Sicherheitsprinzip, das die klassische Vorstellung des „vertrauenswürdigen Netzwerks“ ablöst. Es basiert auf der Annahme, dass kein Gerät, keine Identität und kein Zugriff per se vertrauenswürdig ist. Jeder Zugriff wird kontextbezogen geprüft – anhand von Benutzeridentität, Gerätezustand, Standort und Risiko. In föderalen Verbänden bedeutet das, dass sowohl Haupt- als auch Ehrenamt über gleiche Sicherheitsmaßstäbe verfügen, unabhängig davon, wo oder womit sie sich anmelden.

Die Umsetzung von Zero Trust geschieht über Technologien wie [Active Directory / Entra ID](#active-directory), Conditional Access, Multi-Faktor-Authentifizierung und Gerätemanagement (Intune). Entscheidend ist jedoch der kulturelle Wandel: Sicherheit wird nicht mehr als Barriere erlebt, sondern als Ermöglicher von Vertrauen in einem digitalen Ökosystem. Zero Trust wird so zum verbindenden Prinzip zwischen zentraler Verantwortung und dezentraler Eigenständigkeit.


## Identitätsmanagement (IDM)
{: #identity-management }

Identitätsmanagement ist die Grundlage jeder modernen IT-Architektur. Es beschreibt die Verwaltung digitaler Identitäten, ihrer Attribute, Rollen und Berechtigungen. In einem föderalen Verband übernimmt es die Aufgabe, Menschen, Organisationseinheiten und technische Ressourcen miteinander zu verknüpfen. Wer darf worauf zugreifen? Welche Rolle hat jemand im System? Welche Anwendungen sollen automatisch bereitgestellt werden? – Diese Fragen beantwortet ein gut strukturiertes IDM.

Durch die Kopplung mit [Single Sign-On (SSO)](#sso) entsteht ein durchgängiges Nutzererlebnis über alle Dienste hinweg. Verbände profitieren dabei doppelt: Sie gewinnen Übersicht über Zugriffsrechte und schaffen zugleich Komfort für ihre Nutzer. In Kombination mit [Active Directory / Entra ID](#active-directory) wird Identitätsmanagement zur Schaltzentrale der digitalen Zusammenarbeit – und bildet die Voraussetzung für Konzepte wie [Zero Trust](#zero-trust) oder hybride Infrastrukturen.


## Single Sign-On (SSO)
{: #sso }

Single Sign-On ist das Tor zu einem nahtlosen digitalen Alltag. Statt sich bei jedem Dienst separat anzumelden, authentifizieren sich Nutzer einmal und erhalten Zugriff auf alle freigegebenen Systeme – ob E-Mail, Cloud-Drive oder Videokonferenz. In großen Organisationen reduziert SSO den administrativen Aufwand und minimiert Risiken durch Passwort-Wiederverwendung. Für das Ehrenamt ist es die Eintrittskarte in eine sichere, einheitliche Arbeitsumgebung.

Die technische Basis bildet ein zentrales [Identitätsmanagement](#identity-management), meist in Verbindung mit [Active Directory / Entra ID](#active-directory) oder OpenID-Providern. Doch SSO ist mehr als Bequemlichkeit – es ist eine Brücke zwischen Sicherheit und Nutzerfreundlichkeit. Wenn die Anmeldung gleichzeitig einfach und sicher ist, sinkt die Hemmschwelle, digitale Tools aktiv zu nutzen. In Verbänden kann das über Erfolg oder Scheitern von Digitalprojekten entscheiden.


## Tenant
{: #tenant }

Ein Tenant – also ein Mandant – ist die logische Einheit in Cloud-Umgebungen wie [Microsoft 365](#ms365). Er trennt Daten, Benutzer und Konfiguration voneinander, sodass mehrere Organisationen oder Teilorganisationen sicher in einer gemeinsamen Infrastruktur arbeiten können. Für große Verbände bietet dieses Prinzip den Vorteil, dass der Bundesverband die Gesamtarchitektur kontrolliert, während die Länder eigene Strukturen innerhalb des Systems verwalten.

Technisch gesehen ist der Tenant das Fundament für Governance und Sicherheit. Über ihn lassen sich Policies, Compliance-Regeln und Zugriffsebenen steuern. Durch Integration mit [Zero Trust](#zero-trust)-Mechanismen und abgestuften Admin-Rollen können Verantwortlichkeiten klar abgegrenzt werden. Damit wird der Tenant zu einem organisatorischen Instrument: Er übersetzt die föderale Struktur eines Verbands direkt in die Cloud-Architektur.


## Multitenant
{: #multitenant }

Multitenant bezeichnet die Fähigkeit einer Plattform, mehrere Mandanten parallel zu betreiben – ohne dass sie sich gegenseitig beeinträchtigen. Für Verbände ist das essenziell: Es erlaubt den Ländern, eigene Umgebungen zu verwalten, während sie trotzdem Teil eines einheitlichen Systems bleiben. Jede Organisationseinheit kann eigene Konfigurationen, Gruppen und [Subdomains](#subdomain) nutzen, ohne die zentrale Governance zu verlassen.

Dieses Modell vereint Effizienz und Freiheit. Während der Bundesverband Sicherheits- und Compliance-Richtlinien vorgibt, behalten die Landesverbände ihre operative Selbstständigkeit. Durch abgestufte Berechtigungen im [Active Directory / Entra ID](#active-directory) und einheitliche SSO-Mechanismen bleibt der Gesamtkosmos konsistent – ein Paradebeispiel für technische Standardisierung bei gleichzeitiger Autonomie.


## Subdomain
{: #subdomain }

Subdomains wie *bayern.verband.de* oder *nrw.verband.de* sind weit mehr als Adressen – sie sind Ausdruck organisatorischer Identität. Sie strukturieren Verantwortlichkeiten und schaffen Orientierung in großen föderalen Systemen. Jede Subdomain kann eigene Dienste, Mailkonten oder Admins enthalten, während sie gleichzeitig unter der gemeinsamen Hauptdomain agiert. Das schafft Transparenz, klare Zuständigkeiten und Wiedererkennbarkeit.

In einer [Multitenant](#multitenant)-Architektur dienen Subdomains auch der technischen Trennung von Konfigurationen. So kann etwa jeder Landesverband eigene [Exchange](#exchange)-Richtlinien, Postfächer und Gruppen verwalten. Gleichzeitig stärken sie das gemeinsame Markenbild nach außen – alle bewegen sich im selben digitalen Haus, aber in klar gekennzeichneten Räumen.


## Domain
{: #domain }

Die Domain ist das digitale Aushängeschild einer Organisation. Sie bestimmt, wie E-Mails aussehen, Webseiten erreichbar sind und Identitäten im Internet erscheinen. Eine einheitliche Domain – beispielsweise *verband.de* – bündelt Markenwirkung, Vertrauen und Sicherheit. In Verbänden schafft sie einen sichtbaren Rahmen, innerhalb dessen [Subdomains](#subdomain) und [Tenants](#tenant) wie Unterkapitel eines gemeinsamen Systems agieren.

Aus technischer Sicht ist die Domain oft der Ankerpunkt für Dienste wie [Microsoft 365](#ms365), [SSO](#sso) oder [OpenXchange](#openxchange). Sie definiert, wer „dazugehört“ und bildet damit die Grundlage für Identität im digitalen Raum. Je konsistenter das Domain-Management, desto klarer die Kommunikation – nach innen wie nach außen.


## Active Directory / Entra ID
{: #active-directory }

Das Active Directory – heute als Entra ID weiterentwickelt – ist das Herzstück moderner Identitätsverwaltung. Es dient als zentrales Verzeichnis für Benutzer, Gruppen, Geräte und Zugriffsrechte. In der Cloud-Variante von [Microsoft 365](#ms365) übernimmt es die Steuerung von Rollen, Lizenzen und Sicherheitsrichtlinien. Es bildet damit die Grundlage für Funktionen wie [Single Sign-On (SSO)](#sso), Conditional Access und Multi-Faktor-Authentifizierung. In Verbänden mit vielen Ebenen und Organisationseinheiten schafft Entra ID Transparenz und Nachvollziehbarkeit: Wer darf was, in welcher Rolle und in welchem Kontext?

Besonders in hybriden Szenarien – also der Kombination aus lokaler IT und Cloud-Umgebung – wirkt Entra ID als Brücke. Es verbindet On-Premise-Strukturen mit der Cloud, gleicht Benutzeridentitäten ab und sorgt dafür, dass Berechtigungen aktuell bleiben. In Kombination mit [Zero Trust](#zero-trust) und [Identitätsmanagement (IDM)](#identity-management) wird es zum Rückgrat der digitalen Sicherheitsarchitektur, das Kontrolle und Flexibilität miteinander vereint.


## LDAP
{: #ldap }

LDAP (Lightweight Directory Access Protocol) ist ein standardisiertes Kommunikationsprotokoll, das es Anwendungen ermöglicht, Informationen aus Verzeichnisdiensten wie dem [Active Directory / Entra ID](#active-directory) abzurufen. In föderalen Organisationen kommt LDAP häufig dort zum Einsatz, wo unterschiedliche Systeme miteinander verknüpft werden sollen – etwa zwischen einer Open-Source-Plattform und der Microsoft-Umgebung. Es erlaubt die Synchronisation von Benutzerkonten, Gruppen und Attributen, sodass Identitäten konsistent bleiben.

Gerade in Szenarien, in denen sowohl Hauptamt als auch Ehrenamt mit verschiedenen Systemen arbeiten, ist LDAP ein zentraler Integrationsbaustein. In Kombination mit SCIM-Schnittstellen (System for Cross-Domain Identity Management) lassen sich Provisionierungsprozesse automatisieren. Damit wird LDAP zu einem unsichtbaren, aber unverzichtbaren Bestandteil jeder [Multitenant](#multitenant)-Architektur, die heterogene IT-Landschaften miteinander verbindet.


## Exchange (Online)
{: #exchange }

<a href="https://www.microsoft.com/exchange" target="_blank" rel="noopener">Exchange Online</a> ist das E-Mail- und Kalendersystem innerhalb von [Microsoft 365](#ms365). Es bietet weit mehr als nur Postfächer: Durch Richtlinien, Gruppen und Berechtigungen lässt sich Kommunikation gezielt strukturieren. In föderalen Verbänden ermöglicht ein Rollenmodell mit lokalen Exchange-Admins, dass Länder und Regionen eigenständig agieren können, während der Bundesverband die Gesamtverantwortung behält. Dadurch entsteht eine Balance aus zentraler Governance und dezentraler Handlungsfreiheit.

Technisch ist Exchange eng mit [Active Directory / Entra ID](#active-directory) und dem [Identitätsmanagement (IDM)](#identity-management) verbunden. Gemeinsam bilden sie die Basis für Sicherheit, Nachvollziehbarkeit und organisatorische Klarheit. Ergänzt durch Tools wie [SSO](#sso) und [Zero Trust](#zero-trust)-Mechanismen, wird Exchange Online zum zentralen Kommunikationsknotenpunkt des Verbandes – eine moderne, skalierbare und regelkonforme Kommunikationsplattform.



## Collaboration
{: #collaboration }

Collaboration bezeichnet die Art und Weise, wie Menschen in einer Organisation zusammenarbeiten – technisch, organisatorisch und kulturell. In digitalen Verbänden ist sie weit mehr als der Einsatz von Tools wie Teams, Rocket.Chat oder OpenTalk. Sie umfasst die gemeinsame Informationsarchitektur, klare Rollen, transparente Kommunikationswege und eine Kultur des Teilens. Gute Collaboration entsteht dort, wo Technik nicht Selbstzweck, sondern Ermöglicher ist.

Die technische Basis bilden Plattformen wie [Microsoft 365](#ms365) oder [Open-Source](#opensource)-Lösungen, verbunden durch [SSO](#sso) und ein starkes [Identitätsmanagement (IDM)](#identity-management). Doch entscheidend bleibt der Mensch: Nur wenn Werkzeuge intuitiv und zugänglich sind, entfalten sie ihr Potenzial. Collaboration ist damit auch immer ein Change-Prozess – ein ständiges Lernen, Abstimmen und Neu-Erfinden der eigenen Arbeitsweise.


## Open-Source (OS)
{: #opensource }

Open-Source beschreibt nicht nur eine Lizenzform, sondern eine Haltung: Offenheit, Teilhabe und Selbstbestimmung. Für Verbände mit großem Ehrenamt bietet sie eine realistische Alternative zu kommerziellen Cloud-Lösungen. Systeme wie [OpenXchange](#openxchange), [Rocket.Chat](#rocket-chat) oder [OpenTalk](#opentalk) ermöglichen Datenschutz-konforme Kommunikation, ohne Abhängigkeit von großen Anbietern. Durch eigene Server oder vertrauenswürdige Hosting-Partner behält der Verband die Hoheit über seine Daten – ein wichtiger Baustein digitaler Souveränität.

Gleichzeitig erfordert Open-Source ein hohes Maß an Professionalität. Updates, Monitoring, Backups und Security-Patches müssen zuverlässig umgesetzt werden. In Kombination mit [SSO](#sso) und einem zentralen [Identitätsmanagement](#identity-management) lässt sich eine ebenso komfortable wie sichere Arbeitsumgebung aufbauen. So wird Open-Source zu einer bewussten strategischen Entscheidung – nicht aus Ideologie, sondern aus Verantwortung gegenüber Datenschutz, Nachhaltigkeit und Kosten.


## OpenXchange (OX)
{: #openxchange }

<a href="https://www.open-xchange.com/" target="_blank" rel="noopener">Open-Xchange (OX)</a> ist eine Open-Source-Plattform, die E-Mail, Kalender, Kontakte, Dateifreigabe und Online-Office vereint. Sie bietet eine datenschutzkonforme Alternative zu kommerziellen Cloud-Anbietern und eignet sich besonders für große Nutzerzahlen im Ehrenamt. Über eine gemeinsame [Domain](#domain) und zentrale [SSO](#sso)-Authentifizierung entsteht ein einheitliches Nutzererlebnis – unabhängig davon, wo die Daten physisch liegen. Für viele Verbände ist OX deshalb ein Schlüssel, um digitale Teilhabe sicher und skalierbar zu gestalten.

Ein entscheidender Vorteil liegt in der Integration mit anderen Systemen: OX lässt sich über [LDAP](#ldap) oder SCIM an vorhandene Identitätsquellen anbinden und so in die Gesamtarchitektur einfügen. Kombiniert mit [Rocket.Chat](#rocket-chat) für Chat-Kommunikation und [OpenTalk](#opentalk) für Videokonferenzen entsteht ein vollständiges Open-Source-Ökosystem – eine souveräne digitale Infrastruktur, die in ihrer Gesamtheit dem Verband gehört.



## Rocket.Chat
{: #rocket-chat }

<a href="https://rocket.chat/" target="_blank" rel="noopener">Rocket.Chat</a> ist eine Open-Source-Chat- und Collaboration-Plattform, die Gruppen-, Kanal- und Direktkommunikation ermöglicht. Sie kann eigenständig betrieben oder in hybride Systeme integriert werden – etwa als Bindeglied zwischen der M365-Welt und der Open-Source-Umgebung des Ehrenamts. Über Schnittstellen, Webhooks und APIs lässt sich Rocket.Chat nahtlos mit Tools wie [OpenXchange](#openxchange), [OpenTalk](#opentalk) oder [Microsoft Teams](#collaboration) verknüpfen. Damit wird es zu einer universellen Kommunikationszentrale.

Für Verbände liegt der Vorteil in der Anpassbarkeit. Rollen, Rechte, Themenräume und Integrationen können exakt an die föderale Struktur angepasst werden. Zusammen mit [SSO](#sso) und zentralem [Identitätsmanagement (IDM)](#identity-management) entsteht eine sichere und zugleich offene Kommunikationsumgebung. Rocket.Chat fördert Dialog, Transparenz und Beteiligung – drei Werte, die für das Ehrenamt unverzichtbar sind.



## OpenTalk
{: #opentalk }

<a href="https://opentalk.eu/" target="_blank" rel="noopener">OpenTalk</a> ist eine Open-Source-Videokonferenz-Lösung, entwickelt mit Fokus auf Datenschutz, Stabilität und Skalierbarkeit. Sie bietet alle Funktionen klassischer Videokonferenzsysteme – Meetings, Breakout-Räume, Bildschirmfreigabe – kombiniert mit europäischen Datenschutzstandards. Für den Verband ist OpenTalk besonders attraktiv, weil es sich in bestehende [SSO](#sso)-Strukturen und [Identitätsmanagement (IDM)](#identity-management) integrieren lässt. Damit wird Videokommunikation zu einem nativen Bestandteil der Gesamtplattform – nicht zu einem externen Fremdkörper.

In Kombination mit [Rocket.Chat](#rocket-chat) und [OpenXchange (OX)](#openxchange) entsteht eine vollständige Kommunikationsumgebung für das Ehrenamt. OpenTalk steht exemplarisch für das Prinzip „Souveränität durch Technik“: Kontrolle über Daten, nachhaltige Entwicklung und Unabhängigkeit von proprietären Lösungen. Es ist damit ein Symbol für die digitale Selbstbestimmung, die viele Organisationen anstreben.



---

## Weiterführend – Projektbezug

{% assign term = site.data.glossar | where: "slug", "identity-management" | first %}
{% if term and term.projects %}
  {% assign proj_ids = term.projects %}
  <div class="glossar-grid">
    {% for pid in proj_ids %}
      {% assign p = site.data.projects | where: "id", pid | first %}
      {% if p %}
        {% assign teaser = p.hero.teaser | default: p.hero.image | default: p.seo.image | default: "/assets/images/projects/placeholder-600.webp" %}
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
