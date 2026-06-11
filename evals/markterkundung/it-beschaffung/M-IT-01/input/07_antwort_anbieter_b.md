---
title: "Testakte M-IT-01 – Antwort Anbieter B"
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


# Aktenstück 07 – Antwort Anbieter B: CivicFlow Technologies GmbH

## 1. Einordnung

**Fiktiver Marktteilnehmer:** CivicFlow Technologies GmbH  
**Marktsegment:** Low-Code-/Workflow-Plattform für öffentliche Auftraggeber  
**Eingang der Antwort:** T+8 Wochen  
**Umfang der Antwort:** Strukturierte schriftliche Rückmeldung

## 2. Kurzprofil des Anbieters

CivicFlow Technologies GmbH bietet eine Low-Code-Plattform für digitale Verwaltungsprozesse an. Die Plattform enthält Bausteine für Formulare, Workflows, Rollenmodelle, Fristen, Aufgabensteuerung, Schnittstellen und Auswertungen. Fachliche Prozesslogiken werden projektspezifisch konfiguriert.

## 3. Einschätzung zur fachlichen Abdeckung

Anbieter B weist darauf hin, dass keine fertige Speziallösung für schulbezogene Verwaltungsleistungen angeboten werde. Die Plattform könne die Prozesse aber nach Konfiguration abbilden.

| Bereich | Einschätzung Anbieter B |
|---|---|
| Antragstellung | Plattformstandard |
| Nachweis-Upload | Plattformstandard |
| Statusinformationen | Plattformstandard |
| Sachbearbeitungsworkflow | Plattformstandard, fachlich zu modellieren |
| Mehrmandantenfähigkeit | Plattformstandard |
| Fachregeln | projektspezifisch zu konfigurieren |
| Bescheidvorbereitung | möglich, aber abhängig von Vorlagen und Fachregeln |
| Leihgeräteverwaltung | nur als eigener Prozess oder über Schnittstelle |
| Auswertungen | Standard-Dashboard plus individuelle Berichte |

Anbieter B hält es für realistisch, einen ersten produktiven Pilotprozess innerhalb von 9 bis 12 Monaten umzusetzen, wenn Fachentscheidungen und Schnittstellen frühzeitig geklärt werden.

## 4. Betriebsmodell

Anbieter B bietet drei Betriebsmodelle an:

1. SaaS in EU-Rechenzentren;
2. Private-Cloud-Betrieb für öffentliche Auftraggeber;
3. Betrieb in einem vom Auftraggeber benannten Rechenzentrum.

Der Anbieter weist darauf hin, dass On-Premises-Betrieb mehr Mitwirkung des Auftraggebers, längere Releasezyklen und höhere Betriebskosten verursachen könne.

## 5. Schnittstellen und technische Einbindung

CivicFlow nennt folgende Integrationsmöglichkeiten:

- REST-APIs;
- OIDC/SAML;
- Ereignis- und Nachrichtenqueues;
- CSV/XML-Importe;
- optionale Adapterentwicklung für Altsysteme.

Zum `DMS-Nord` und zu `SchulFach 9` könne ohne technische Detailunterlagen keine belastbare Aussage getroffen werden. Eine vorgelagerte Schnittstellenanalyse sei erforderlich.

## 6. Datenportabilität und Konfiguration

Anbieter B betont, dass Prozessmodelle, Formulare und Rollenmodelle grundsätzlich exportiert werden können. Der Export erfolge jedoch in einem plattformeigenen JSON-Format. Eine vollständige Übertragbarkeit auf andere Low-Code-Plattformen könne nicht zugesichert werden.

Datenexporte seien in CSV, JSON und über API möglich. Dokumente könnten in Originalformaten und zusätzlich als PDF/A exportiert werden.

## 7. Datenschutz und IT-Sicherheit

Anbieter B verweist auf folgende Maßnahmen:

- mandantenfähiges Rollen- und Rechtemodell;
- Protokollierung von administrativen Aktionen;
- Verschlüsselung bei Transport und Speicherung;
- AVV nach Art. 28 DSGVO;
- getrennte Test- und Produktivumgebungen;
- Security-Patching nach definierten Releasezyklen.

Der Anbieter empfiehlt für die geplanten Datenarten eine Datenschutz-Folgenabschätzung vor Produktivsetzung zu prüfen.

## 8. Barrierefreiheit

Die Standardoberflächen sollen WCAG 2.1 AA unterstützen. Der Anbieter weist darauf hin, dass Barrierefreiheit bei Low-Code-Konfigurationen wesentlich von der Modellierung, den Formularen und den eingebundenen Dokumenten abhängt.

## 9. KI-Funktionen

CivicFlow bietet optionale KI-Assistenzfunktionen über separate Module an. Genannt werden:

- Klassifikation hochgeladener Dokumente;
- Formulierungsvorschläge für Rückfragen;
- Zusammenfassung längerer Freitextangaben;
- interne Wissensassistenz für Sachbearbeitung.

Der Anbieter empfiehlt, KI-Funktionen nicht in die erste Produktivstufe aufzunehmen, sondern erst nach Stabilisierung der Kernprozesse und nach Datenschutz-/Risikoprüfung zu pilotieren.

## 10. Kosten- und Aufwandskorridor

| Kostenblock | Unverbindlicher Korridor netto |
|---|---:|
| Plattformkonfiguration und Prozessmodellierung | 350.000–650.000 EUR |
| Schnittstellenanalyse und Adapter | 180.000–420.000 EUR |
| Migration | 80.000–220.000 EUR |
| Schulung / Enablement Auftraggeber | 70.000–160.000 EUR |
| Lizenz und Betrieb pro Jahr | 160.000–300.000 EUR |

Anbieter B weist darauf hin, dass die Kosten stark davon abhängen, ob die AöR eigene Prozessverantwortliche und geschulte Plattform-Administratoren aufbaut.

## 11. Hinweise des Anbieters

Aus Sicht von Anbieter B sollte die spätere Ausschreibung nicht zu stark auf ein Fachportal zugeschnitten werden. Entscheidend seien funktionale Anforderungen, Schnittstellen, Rollenmodell, Datenportabilität, Betriebsmodell und eindeutige Mitwirkungspflichten.
