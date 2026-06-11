---
title: "Testakte M-IT-01 – Antwort Anbieter D"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "market-response"
eval_role: "input"
eval_case_id: "M-IT-01"
relative_date: "T+8 Wochen"
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


# Aktenstück 09 – Antwort Anbieter D: SchulFach Digital GmbH

## 1. Einordnung

**Fiktiver Marktteilnehmer:** SchulFach Digital GmbH  
**Marktsegment:** Hersteller des bestehenden Fachverfahrens `SchulFach 9`  
**Eingang der Antwort:** T+8 Wochen  
**Umfang der Antwort:** Schriftliche Rückmeldung mit Angebot eines vertiefenden Konzeptgesprächs

## 2. Kurzprofil des Anbieters

SchulFach Digital GmbH ist Herstellerin des bei der AöR eingesetzten Altverfahrens `SchulFach 9`. Nach eigener Darstellung betreut sie mehrere kommunale Kunden mit schulbezogenen Fachprozessen.

## 3. Einschätzung zum Lösungsansatz

Anbieter D schlägt vor, das bestehende Fachverfahren `SchulFach 9` um ein externes Portalmodul zu erweitern. Die Lösung solle eng an die bestehende Datenstruktur und Sachbearbeitungslogik angebunden werden.

Aus Sicht des Anbieters sei dies der schnellste und risikoärmste Weg, weil Datenmodell, Rollenlogik und Fachhistorie bereits bekannt seien. Der Anbieter hält eine Ablösung oder parallele Einführung eines separaten Portals für aufwändig und fehleranfällig.

## 4. Fachliche Abdeckung

Anbieter D gibt an, folgende Leistungen mit vorhandenen oder kurzfristig verfügbaren Modulen abbilden zu können:

- Schülerbeförderung;
- Lernmittelfreiheit;
- Zuschüsse zur Mittagsverpflegung;
- Härtefallanträge;
- Statusinformationen;
- Upload von Nachweisen;
- interne Prüf- und Freigabeprozesse.

Für die Leihgeräteverwaltung verweist Anbieter D auf ein Zusatzmodul, das noch nicht allgemein verfügbar sei. Eine Auslieferung könne im Projekt erfolgen.

## 5. Betriebsmodell

Anbieter D bietet zwei Betriebsmodelle an:

1. Betrieb im bisherigen technischen Umfeld der AöR;
2. Hosting in einer vom Anbieter benannten EU-Umgebung.

Ein Betrieb auf einer beliebigen Cloudplattform oder in einer vom Auftraggeber frei gewählten Containerumgebung sei nicht vorgesehen. Der Anbieter begründet dies mit Supportfähigkeit, Produkthaftung und Releasekontrolle.

## 6. Schnittstellen und Datenportabilität

Anbieter D verweist darauf, dass die tiefste Integration mit `SchulFach 9` nur über proprietäre Schnittstellen möglich sei. Standardisierte Exporte seien für Vorgangsdaten, Bescheiddaten und Dokumentenmetadaten verfügbar.

Workflow-Regeln, Formularlogiken und bestimmte Fachregeln seien Bestandteil des Produkts und könnten nicht vollständig in offenen Formaten exportiert werden.

Eine DMS-Anbindung sei möglich, wenn die AöR die technischen Spezifikationen und Testzugänge bereitstelle. Zum Formularserver des Landesportals empfiehlt Anbieter D, zunächst auf eine direkte Anbindung zu verzichten und stattdessen das eigene Portalmodul zu nutzen.

## 7. Datenschutz und IT-Sicherheit

Anbieter D verweist auf bestehende Sicherheitsmechanismen des Fachverfahrens und auf Erfahrungen mit kommunalen Sozial- und Schuldaten. Ein Datenschutzkonzept könne im Rahmen eines Feinkonzepts erstellt werden.

Eine Datenschutz-Folgenabschätzung hält der Anbieter nur dann für erforderlich, wenn neue KI-Funktionen oder umfassende Profilbildungen eingeführt werden. Nähere Ausführungen zu Löschkonzept, Protokollierung und Mandantentrennung werden nicht gemacht.

## 8. Barrierefreiheit

Anbieter D gibt an, das Portalmodul orientiere sich an WCAG-Anforderungen. Eine externe Barrierefreiheitsprüfung sei bislang nicht Bestandteil des Standardangebots, könne aber optional beauftragt werden.

## 9. KI-Funktionen

Anbieter D bietet derzeit keine produktiven KI-Funktionen für das Portalmodul an. Für eine spätere Ausbaustufe sei ein Modul zur automatischen Dokumentenerkennung geplant. Details zur Datenverarbeitung und zum Betriebsmodell liegen nach Anbieterangabe noch nicht vor.

## 10. Kosten- und Aufwandskorridor

| Kostenblock | Unverbindlicher Korridor netto |
|---|---:|
| Erweiterung `SchulFach 9` um Portalmodul | 300.000–520.000 EUR |
| Einrichtung und Parametrisierung | 120.000–240.000 EUR |
| Migration / Datenbereinigung | 80.000–180.000 EUR |
| DMS-Anbindung | 80.000–180.000 EUR |
| Betrieb und Pflege pro Jahr | 140.000–260.000 EUR |

Anbieter D weist darauf hin, dass diese Größenordnungen nur gelten, wenn das vorhandene Fachverfahren als führendes System bestehen bleibt und keine umfangreichen offenen Schnittstellen oder parallelen Plattformmodelle verlangt werden.

## 11. Angebot eines Feinkonzepts

Anbieter D bietet an, kurzfristig ein vertiefendes Feinkonzept mit Zielarchitektur, Einführungspfad und Aufwandsschätzung zu erstellen. Das Konzept könne kostenfrei erstellt werden, wenn die AöR zusichert, den Anbieter bei einer späteren Beschaffung einzubeziehen.

Der Anbieter weist darauf hin, dass das Konzept urheberrechtlich geschützt sei und ohne Zustimmung nicht in Vergabeunterlagen übernommen werden dürfe.

## 12. Hinweise des Anbieters

Anbieter D hält eine Gesamtvergabe für zwingend vorzugswürdig. Eine Losbildung in Portal, Schnittstellen, Betrieb und Migration sieht der Anbieter kritisch, da dadurch Verantwortlichkeiten aufgespalten und Projektrisiken erhöht würden.
