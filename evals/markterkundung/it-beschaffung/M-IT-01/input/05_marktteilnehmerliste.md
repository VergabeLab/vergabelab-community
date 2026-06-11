---
title: "Testakte M-IT-01 – Marktteilnehmerliste und Ansprachekonzept"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "market-participant-list"
eval_role: "input"
eval_case_id: "M-IT-01"
relative_date: "T+3 Wochen"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/markterkundung/it-beschaffung/M-IT-01/input"

module_id: "markterkundung-it-beschaffung"
module: "markterkundung"
procurement_area: "it-beschaffung"

related_skill: "agent-skills/markterkundung-it-beschaffung"
related_custom_gpt_prompt: "prompts/markterkundung/it-beschaffung/01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md"

target_systems:
  - "chatgpt-custom-gpt"
  - "claude-skill"
  - "generic-llm"

spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
---

<!-- SPDX-FileCopyrightText: 2026 Okan Doğan -->
<!-- SPDX-License-Identifier: CC-BY-4.0 -->


# Aktenstück 05 – Marktteilnehmerliste und Ansprachekonzept

## 1. Zweck des Dokuments

Dieses Aktenstück dokumentiert, welche fiktiven Marktteilnehmer für die Markterkundung in Betracht gezogen werden und aus welchen Gründen sie ausgewählt wurden.

Die Liste stellt **keine Vorauswahl für ein späteres Vergabeverfahren** dar. Sie dient lediglich dazu, unterschiedliche Marktsegmente abzudecken und ein möglichst breites Bild zu Lösungsansätzen, Betriebsmodellen, Schnittstellen, Migration, Kostenstrukturen und Risiken zu erhalten.

## 2. Auswahlgrundsätze

Die Vergabestelle möchte unterschiedliche Lösungsansätze erfassen:

- Fachportal oder standardisierte Branchenlösung;
- Low-Code-/Workflow-Plattform;
- Open-Source- oder modularer Integrationsansatz;
- Erweiterung des bestehenden Altverfahrens.

Alle angeschriebenen Marktteilnehmer sollen dieselben Informationen erhalten. Individuelle Zusatzinformationen, Produktdemos oder bilaterale Konzeptgespräche sollen nur stattfinden, wenn sie dokumentiert und diskriminierungsfrei behandelt werden können.

## 3. Vorgesehene Marktteilnehmer

| Kürzel | Fiktiver Marktteilnehmer | Marktsegment | Grund für Ansprache |
|---|---|---|---|
| Anbieter A | NordPortal Solutions GmbH | Standardnahes Fachportal für kommunale Verwaltungsleistungen | Marktbekannter Ansatz für digitale Antrags- und Vorgangsbearbeitung; mögliche Abdeckung mehrerer schulbezogener Prozesse |
| Anbieter B | CivicFlow Technologies GmbH | Low-Code-/Workflow-Plattform für öffentliche Auftraggeber | Alternative zu Fachportal und Individualentwicklung; relevant für Wiederverwendbarkeit und schnelle Prozesskonfiguration |
| Anbieter C | OpenGov Werkstatt eG | Open-Source-nahe Integrations- und Portalentwicklung | Relevanz für Datenportabilität, offene Schnittstellen, Nachnutzung und Vermeidung von Lock-in |
| Anbieter D | SchulFach Digital GmbH | Hersteller des bestehenden Fachverfahrens `SchulFach 9` | Bestehender Systembezug; mögliche Erweiterung des Altverfahrens; zugleich erhöhtes Risiko eines Produkt- oder Herstellerzuschnitts |

## 4. Besondere Hinweise zu Anbieter D

Anbieter D ist der Hersteller des vorhandenen Fachverfahrens `SchulFach 9`. Ein Mitarbeitender des Anbieters hat dem Fachbereich informell angeboten, kostenfrei ein Grobkonzept zu erstellen, sofern der Anbieter später in das Verfahren einbezogen wird.

Die Vergabestelle hat hierzu vermerkt:

- Eine privilegierte Informationsgabe an Anbieter D ist zu vermeiden.
- Ein kostenfreies Konzept darf nicht ohne Prüfung der Gleichbehandlung, Dokumentation und Verwertbarkeit angenommen werden.
- Wenn Informationen aus Gesprächen mit Anbieter D in spätere Vergabeunterlagen einfließen, muss geprüft werden, ob dadurch Wettbewerbsvorteile entstehen oder Know-how einseitig übernommen wird.
- Anbieter D darf nicht ausgeschlossen werden, nur weil er Altanbieter ist; eine etwaige Vorbefassung muss aber transparent behandelt und erforderlichenfalls ausgeglichen werden.

## 5. Vorgesehenes Anspracheverfahren

Die Vergabestelle erwägt folgendes Vorgehen:

1. Versand eines neutralen Anschreibens mit identischem Informationsstand an alle vier Marktteilnehmer.
2. Rückmeldefrist von drei Wochen.
3. Keine verbindlichen Preisangebote, sondern strukturierte Kosten- und Aufwandskorridore.
4. Keine Bewertung oder Rangfolge der Rückmeldungen.
5. Dokumentation aller eingegangenen Antworten in einer neutralen Synopse.
6. Prüfung, ob weitere Marktteilnehmer oder Veröffentlichungswege einbezogen werden sollten, falls die Rückmeldungen zu einseitig ausfallen.
7. Keine Übernahme anbieterspezifischer Formulierungen in spätere Vergabeunterlagen ohne Neutralisierung und Dokumentation.

## 6. Interne offene Punkte zur Ansprache

- Soll die Markterkundung nur durch direkte Ansprache der vier Anbieter erfolgen oder zusätzlich öffentlich auf der Vergabeplattform angekündigt werden?
- Welche Informationen zum Budgetrahmen dürfen mitgeteilt werden, ohne Preissteuerung auszulösen?
- Soll eine einheitliche Antwortmatrix vorgegeben werden?
- Wie wird mit Unterlagen umgegangen, die Anbieter als vertraulich kennzeichnen?
- Sollen Produktdemos zugelassen werden, und falls ja, unter welchen Dokumentations- und Gleichbehandlungsbedingungen?
