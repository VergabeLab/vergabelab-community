---
title: "Testakte M-IT-01 – Antwort Anbieter C"
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


# Aktenstück 08 – Antwort Anbieter C: OpenGov Werkstatt eG

## 1. Einordnung

**Fiktiver Marktteilnehmer:** OpenGov Werkstatt eG  
**Marktsegment:** Open-Source-nahe Integrations- und Portalentwicklung  
**Eingang der Antwort:** T+8 Wochen  
**Umfang der Antwort:** Schriftliche Rückmeldung mit Architekturhinweisen

## 2. Kurzprofil des Anbieters

OpenGov Werkstatt eG beschreibt sich als Anbieterin für modulare Verwaltungsportale, offene Schnittstellen und Integrationsarchitekturen. Die Genossenschaft entwickelt auf Basis quelloffener Komponenten und übernimmt Konzeption, Implementierung, Integration und Betriebsbegleitung.

## 3. Einschätzung zum Lösungsansatz

Anbieter C bietet kein fertiges Fachprodukt für schulbezogene Verwaltungsleistungen an. Vorgeschlagen wird eine modulare Architektur mit folgenden Bausteinen:

- Formular-Frontend;
- Nutzerkonto-/IdP-Anbindung;
- Workflow-Engine;
- Dokumentenablage über DMS-Schnittstelle;
- Fachlogikmodule für einzelne Leistungen;
- Schnittstellen- und Integrationsschicht;
- Auswertungs- und Reportingmodul.

Nach Einschätzung des Anbieters eignet sich dieser Ansatz, wenn Datenportabilität, offene Schnittstellen, Nachnutzung und Vermeidung von Herstellerabhängigkeit besonders wichtig sind. Er erfordere aber eine stärkere fachliche Steuerung durch die AöR.

## 4. Fachliche Abdeckung

Anbieter C kann die beschriebenen Prozesse nach eigener Einschätzung vollständig abbilden, jedoch nicht als Standardprodukt. Der Anbieter empfiehlt, mit zwei bis drei priorisierten Leistungen zu starten, etwa Schülerbeförderung, Lernmittelfreiheit und Leihgeräteverwaltung.

Eine Big-Bang-Einführung aller Leistungen wird ausdrücklich nicht empfohlen.

## 5. Betriebsmodell

Mögliche Betriebsmodelle:

- Betrieb im kommunalen Rechenzentrum;
- Betrieb durch einen öffentlichen IT-Dienstleister;
- Private-Cloud-Betrieb in EU-Rechenzentren;
- Managed Betrieb durch Anbieter C mit Unterauftragnehmern.

SaaS im engeren Sinne wird nicht als Hauptmodell angeboten. Anbieter C hält einen Betrieb in einer kontrollierten Umgebung des Auftraggebers oder eines öffentlichen IT-Dienstleisters für vorzugswürdig.

## 6. Schnittstellen und Datenportabilität

Anbieter C legt den Schwerpunkt auf offene Schnittstellen und Exit-Fähigkeit:

- REST-APIs;
- OIDC/SAML;
- Dokumentenexporte in Originalformaten und PDF/A;
- Metadatenexporte in JSON/XML;
- Workflowmodellierung möglichst in BPMN-naher Form;
- Datenbankexporte und technische Dokumentation als Vertragsbestandteil.

Für `DMS-Nord`, `SchulFach 9`, Formularserver und E-Payment sei jeweils eine technische Vorprüfung erforderlich. Anbieter C empfiehlt, eine separate Schnittstellen- und Migrationsanalyse als frühen Projektbaustein vorzusehen.

## 7. Datenschutz und IT-Sicherheit

Anbieter C weist darauf hin, dass wegen Kinder-, Sozial- und möglichen Gesundheitsdaten ein Datenschutz- und Sicherheitskonzept nicht nur als Anbieterstandard, sondern projektbezogen erstellt werden müsse.

Genannt werden insbesondere:

- Rollen- und Berechtigungskonzept;
- Protokollierung und Löschkonzept;
- Trennung der Mandanten;
- Ende-zu-Ende-Betrachtung der Datenflüsse;
- Verzicht auf unnötige Tracking- und Analysedienste;
- Sicherheitskonzept für externe Zugriffe von Schulen und Dienstleistern.

## 8. Barrierefreiheit

Anbieter C empfiehlt, Barrierefreiheit als verbindliche Abnahmeanforderung zu formulieren und nicht nur als allgemeine Zusicherung. Möglich seien externe Tests gegen BITV-/WCAG-Anforderungen sowie redaktionelle Vorgaben für barrierefreie Formulare und Dokumente.

## 9. KI-Funktionen

Anbieter C rät dazu, KI-Funktionen zunächst nicht zum Kerngegenstand der ersten Beschaffung zu machen. Dokumentenklassifikation und Textvorschläge könnten später als separate optionale Module geprüft werden. Chatbots für Sorgeberechtigte hält Anbieter C wegen möglicher Fehlkommunikation und besonderer Schutzbedürftigkeit der Betroffenen für risikobehaftet.

## 10. Kosten- und Aufwandskorridor

| Kostenblock | Unverbindlicher Korridor netto |
|---|---:|
| Fach- und Architekturkonzeption | 120.000–220.000 EUR |
| Entwicklung Portal/Workflow erste Ausbaustufe | 450.000–800.000 EUR |
| Schnittstellen und Migration | 220.000–500.000 EUR |
| Barrierefreiheits- und Sicherheitsprüfungen | 60.000–140.000 EUR |
| Betrieb und Wartung pro Jahr | 220.000–360.000 EUR |

Der Anbieter weist darauf hin, dass geringere Lizenzkosten nicht automatisch zu geringeren Gesamtkosten führen. Die Projektsteuerung und Mitwirkung des Auftraggebers seien bei einem modularen Ansatz besonders relevant.

## 11. Hinweise des Anbieters

Anbieter C hält eine Losbildung grundsätzlich für möglich, etwa in:

- Portal/Workflow und Fachmodule;
- Schnittstellen/Migration;
- Betrieb;
- Barrierefreiheits- und Sicherheitsprüfung.

Der Anbieter weist zugleich darauf hin, dass Schnittstellen- und Integrationsverantwortung eindeutig geregelt werden müsse.
