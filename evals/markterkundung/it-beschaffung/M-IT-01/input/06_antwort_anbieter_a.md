---
title: "Testakte M-IT-01 – Antwort Anbieter A"
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


# Aktenstück 06 – Antwort Anbieter A: NordPortal Solutions GmbH

## 1. Einordnung

**Fiktiver Marktteilnehmer:** NordPortal Solutions GmbH  
**Marktsegment:** Standardnahes Fachportal für kommunale Verwaltungsleistungen  
**Eingang der Antwort:** T+8 Wochen  
**Umfang der Antwort:** Strukturierte schriftliche Rückmeldung, keine Produktdemo

## 2. Kurzprofil des Anbieters

NordPortal Solutions GmbH beschreibt sich als Anbieterin eines modularen Portals für kommunale Antrags- und Vorgangsbearbeitung. Die Lösung werde in mehreren Kommunalverwaltungen für Leistungen mit Nachweis-Upload, Rückfragen, Statusanzeigen und Bescheidvorbereitung eingesetzt.

## 3. Einschätzung zur fachlichen Abdeckung

Anbieter A gibt an, die beschriebenen Prozesse mit einem vorhandenen Standardprodukt teilweise abbilden zu können.

| Bereich | Einschätzung Anbieter A |
|---|---|
| Digitale Antragstellung | Standardfunktion vorhanden |
| Upload und Nachforderung von Nachweisen | Standardfunktion vorhanden |
| Statusinformationen für Antragstellende | Standardfunktion vorhanden |
| Sachbearbeitungsworkflow | Standardfunktion vorhanden, aber pro Leistung zu konfigurieren |
| Schülerbeförderung | Fachliche Templates teilweise vorhanden |
| Lernmittelfreiheit | Als Verwaltungsleistung abbildbar, aber ohne spezielles Fachmodul |
| Mittagsverpflegung / Zuschüsse | Als Verwaltungsleistung abbildbar |
| Leihgeräteverwaltung | Nur mit Anpassung oder Schnittstelle zu Bestandssystem |
| Härtefallprüfung | Abbildbar, aber stark abhängig vom Regelwerk der AöR |
| Bescheidvorbereitung | Standardfunktion vorhanden; keine vollständig automatisierte Ablehnung |

Anbieter A schätzt, dass etwa **60 bis 75 %** der Anforderungen standardnah abgedeckt werden könnten. Der genaue Anteil hänge von den Fachregeln, Formularen, Rollenmodellen und Schnittstellen ab.

## 4. Betriebsmodell

Anbieter A bietet vorrangig SaaS-Betrieb in ISO-27001-zertifizierten Rechenzentren innerhalb der EU an. Ein Betrieb in einem kommunalen Rechenzentrum sei grundsätzlich möglich, werde aber nur für größere Projekte angeboten und verursache zusätzlichen Betriebs- und Releaseaufwand.

Zum Datenschutz teilt Anbieter A mit:

- Auftragsverarbeitungsvertrag nach Art. 28 DSGVO möglich;
- Mandantentrennung technisch und organisatorisch vorgesehen;
- Protokollierung von Zugriffen und Rollenänderungen;
- keine Nutzung von Kundendaten zum Training von KI-Modellen;
- Drittstaatentransfers sollen nach Anbieterangabe nicht stattfinden, sofern keine externen Zusatzdienste beauftragt werden.

## 5. Schnittstellen und Migration

Anbieter A nennt folgende Schnittstellenmöglichkeiten:

- OIDC/SAML für Identity Provider;
- REST-API für DMS-Anbindung;
- CSV- und XML-Exporte für Fachverfahren;
- Webhook-basierte Benachrichtigungen;
- optionaler XÖV-naher Datenaustausch, jedoch nur nach projektspezifischer Prüfung.

Zur Migration weist Anbieter A darauf hin, dass Altdaten aus `SchulFach 9` nur dann strukturiert übernommen werden können, wenn die Datenfelder, Bereinigungspflichten und Migrationsregeln frühzeitig geklärt werden.

## 6. Datenportabilität und Exit

Anbieter A bietet Exporte von Antragsdaten, Dokumentenmetadaten und Vorgangsstatus in CSV, JSON und PDF/A an. Workflow-Definitionen und Formularlogiken können nach Anbieterangabe dokumentiert, aber nicht vollständig in einem offenen Standard exportiert werden.

Ein Exit-Projekt am Vertragsende sei üblich und müsse gesondert beauftragt werden.

## 7. Barrierefreiheit

Anbieter A gibt an, die Portaloberfläche an WCAG 2.1 AA auszurichten. Eine projektbezogene BITV-Prüfung könne durchgeführt werden. Nicht alle individuell konfigurierten Formulare seien automatisch barrierefrei; hierfür sei eine Qualitätssicherung im Einführungsprojekt erforderlich.

## 8. KI-Funktionen

Anbieter A bietet optionale Assistenzfunktionen an:

- automatische Dokumentenklassifikation;
- Vorschläge für Antworttexte;
- Erkennung fehlender Nachweise;
- Chatbot für allgemeine Fragen zum Verfahrensstand.

Der Anbieter betont, dass diese Funktionen nicht für vollautomatisierte ablehnende Entscheidungen vorgesehen seien. Der Einsatz müsse gesondert datenschutzrechtlich und fachlich bewertet werden.

## 9. Kosten- und Aufwandskorridor

Anbieter A nennt unverbindlich folgende Größenordnungen:

| Kostenblock | Unverbindlicher Korridor netto |
|---|---:|
| Einführung und Konfiguration | 420.000–620.000 EUR |
| Schnittstellen und Migration | 180.000–360.000 EUR |
| Schulung und Change-Begleitung | 60.000–120.000 EUR |
| Betrieb und Support pro Jahr | 180.000–280.000 EUR |
| Optionales Exit-Paket | 40.000–90.000 EUR |

Ein belastbarer Festpreis könne erst nach fachlicher Detailklärung, Schnittstellenanalyse und Migrationsbewertung genannt werden.

## 10. Hinweise des Anbieters

Anbieter A hält eine Gesamtvergabe für organisatorisch einfacher, sieht aber eine fachliche Trennung von Portal/Workflow, Migration/Schnittstellen und Betrieb als grundsätzlich möglich an. Eine zu starke Losbildung könne nach Anbieteransicht Integrationsrisiken erhöhen.
