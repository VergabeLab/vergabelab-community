---
title: "Testakte M-IT-01 – Scoring Rubric"
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "scoring-rubric"
eval_role: "expected"
eval_case_id: "M-IT-01"
relative_date: "T+10 Wochen (interne Auswertung; nicht Teil des Assistenten-Inputs)"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/markterkundung/it-beschaffung/M-IT-01/expected"

module: "markterkundung"
domain: "it-beschaffung"

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


# Aktenstück 12 – Scoring Rubric

## 1. Zweck dieses Dokuments

Dieses Bewertungsraster dient der strukturierten Evaluation von Antworten eines Assistenten auf die Testakte M-IT-01. Es darf bei Blindtests nicht als Input in den Assistenten geladen werden.

Die Bewertung kann je nach Testmodus angepasst werden. Maßgeblich ist nicht, ob der Assistent exakt die gleiche Struktur verwendet, sondern ob er die fachlichen Kernleistungen erreicht.

## 2. Bewertung Test 1 – Aktenanalyse vor Durchführung der Markterkundung

**Maximalpunktzahl: 100 Punkte**

| Kriterium | Punkte | Erwartung |
|---|---:|---|
| Vergaberechtliches Grundverständnis | 20 | Markterkundung als zulässiges Vorbereitungsinstrument; keine Anbieterwahl; Neutralität, Gleichbehandlung und Dokumentation |
| Erkennung offener Informationsbedarfe | 15 | fachliche, technische, wirtschaftliche und rechtliche Informationslücken werden strukturiert erkannt |
| Risikoerkennung | 25 | Produktdemo, Altanbieter, Budgetkommunikation, Datenschutz, IT-Sicherheit, Schnittstellen, Migration, Lock-in und KI werden adressiert |
| Praktische nächste Schritte | 20 | sinnvoller Ablauf: Entwurf bereinigen, Fragenkatalog, gleiche Informationsbasis, Synopse, Dokumentation |
| Trennung der Ebenen | 10 | klare Trennung von Bedarf, Markterkenntnis, späterer Leistungsbeschreibung und Zuschlagswertung |
| Verständlichkeit und Nutzbarkeit | 10 | klare, verwertbare Darstellung für Vergabestelle und Projektgruppe |

## 3. Bewertung Test 2 – Anschreiben und Fragenkatalog

**Maximalpunktzahl: 100 Punkte**

| Kriterium | Punkte | Erwartung |
|---|---:|---|
| Neutralität des Anschreibens | 20 | keine Produkt-, Hersteller-, Technologie- oder Anbieterpräferenz; keine Vorteilszusage |
| Korrekte Abgrenzung der Markterkundung | 15 | keine Angebotsaufforderung, keine Wertung, keine spätere Bevorzugung |
| Bereinigung riskanter Formulierungen | 20 | problematische Punkte aus Aktenstück 04 werden erkannt und entfernt |
| Qualität des Fragenkatalogs | 25 | offene, funktionale und verwertbare Fragen zu Lösung, Schnittstellen, Migration, Betrieb, Datenschutz, Sicherheit, Barrierefreiheit, KI, Kosten, Losbildung |
| Umgang mit Kosten und Budget | 10 | nur unverbindliche Korridore/Kostentreiber; keine Preissteuerung |
| Dokumentationsfähigkeit | 10 | Antworten sind später synopsenfähig und neutral auswertbar |

## 4. Bewertung Test 3 – Auswertung der Marktrückläufe

**Maximalpunktzahl: 100 Punkte**

| Kriterium | Punkte | Erwartung |
|---|---:|---|
| Neutrale Synopse | 20 | Anbieterantworten werden vergleichbar strukturiert, ohne Rangfolge |
| Marktbild | 20 | mehrere Lösungsansätze werden herausgearbeitet; kein Ansatz wird vorschnell bevorzugt |
| Belastbare Erkenntnisse | 15 | Schnittstellen, Migration, Betrieb, Datenportabilität, KI und Kosten werden differenziert ausgewertet |
| Trennung von Erkenntnis und Einzelmeinung | 15 | Anbieterbehauptungen werden nicht unkritisch als Tatsache übernommen |
| Vergaberechtliche Verwertbarkeit | 15 | Erkenntnisse werden neutral für Leistungsbeschreibung, Losbildung, Eignung, Zuschlagskriterien und Vertrag nutzbar gemacht |
| Risiko- und Folgeschrittanalyse | 15 | offene Klärungspunkte und nächste Schritte werden präzise benannt |

## 5. Bewertung Test 4 – Dokumentationsvermerk

**Maximalpunktzahl: 100 Punkte**

| Kriterium | Punkte | Erwartung |
|---|---:|---|
| Zweck und Ausgangslage | 15 | Anlass, Bedarf und Ziel der Markterkundung sind nachvollziehbar dokumentiert |
| Vorgehen | 15 | angesprochene Marktsegmente, gleiche Informationsbasis und Rückmeldeweg sind beschrieben |
| Erkenntnisse | 25 | wesentliche Markterkenntnisse werden neutral und strukturiert zusammengefasst |
| Risikodokumentation | 20 | Produktzuschnitt, Altanbieter, Datenschutz, Schnittstellen, Migration, Lock-in und KI werden dokumentiert |
| Abgrenzung zur Wertung | 15 | keine Anbieterentscheidung, keine Rangfolge, keine Zuschlagsnähe |
| Folgeschritte | 10 | konkrete Überleitung in Leistungsbeschreibung, Losbildung, Vertragsmodell und weitere Prüfungen |

## 6. Kritische KO-Fehler

Unabhängig von der Punktzahl sollte eine Antwort kritisch bewertet werden, wenn sie einen der folgenden Fehler enthält:

- Auswahl oder Empfehlung eines bestimmten Anbieters als Ergebnis der Markterkundung;
- Aussage, ein späteres Vergabeverfahren könne auf Grundlage der Markterkundung zugunsten eines bestimmten Anbieters zugeschnitten werden;
- Übernahme anbieterspezifischer Produktmerkmale als Mindestanforderung ohne Neutralisierung;
- Behandlung der Rückmeldungen als verbindliche Angebote;
- fehlende Erkennung des Altanbieter-/Vorbefassungsrisikos;
- Ignorieren der besonderen Datenschutzrisiken;
- pauschaler Ausschluss von Cloud, Low-Code, Open Source oder Altanbieter ohne Einzelfallbegründung;
- Vermischung von Markterkundung, Eignungsprüfung, Zuschlagswertung und Beschaffungsentscheidung.

## 7. Bewertungsskala (experimentell!)

| Punkte | Einordnung |
|---:|---|
| 90–100 | sehr gut; fachlich belastbar und praktisch unmittelbar verwertbar |
| 75–89 | gut; kleinere Lücken oder Unschärfen, aber insgesamt praxistauglich |
| 60–74 | brauchbar; relevante Punkte erkannt, aber mit deutlichen Lücken |
| 40–59 | kritisch; wesentliche Risiken oder vergaberechtliche Trennlinien fehlen |
| 0–39 | nicht ausreichend; Antwort gefährdet Neutralität, Dokumentation oder spätere Vergaberechtskonformität |
