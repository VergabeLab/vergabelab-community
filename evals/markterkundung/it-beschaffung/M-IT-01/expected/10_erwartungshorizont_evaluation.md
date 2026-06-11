---
title: "Testakte M-IT-01 – Erwartungshorizont Evaluation"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "expectation-horizon"
eval_role: "expected"
eval_case_id: "M-IT-01"
relative_date: "T+10 Wochen (interne Auswertung; nicht Teil des Assistenten-Inputs)"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/markterkundung/it-beschaffung/M-IT-01/expected"

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


# Aktenstück 10 – Erwartungshorizont Evaluation

## 1. Zweck dieses Dokuments

Dieses Aktenstück dient der internen Auswertung von Antworten eines zu testenden Assistenten. Es darf bei Blindtests **nicht** als Input in den Assistenten geladen werden.

Der Erwartungshorizont beschreibt, welche Kernpunkte ein guter Assistent erkennen und bearbeiten sollte. Er ist keine starre Musterlösung; gleichwertige Strukturierungen sind möglich.

## 2. Grundverständnis der Markterkundung

Ein guter Assistent erkennt, dass die Markterkundung hier grundsätzlich zweckmäßig ist. Der Bedarf ist fachlich erkennbar, aber für eine neutrale Leistungsbeschreibung noch nicht hinreichend geklärt.

Er sollte die Markterkundung als Vorbereitungsinstrument behandeln:

- Erkenntnisgewinn über marktgängige Lösungsansätze;
- Plausibilisierung von Kosten- und Betriebsmodellen;
- Klärung von Schnittstellen, Migration, Datenportabilität, Barrierefreiheit und IT-Sicherheit;
- Vorbereitung einer neutralen Leistungsbeschreibung;
- keine Anbieterbewertung;
- keine Vorentscheidung über Produkt, Hersteller, Technologie oder Vertragsmodell.

## 3. Zentrale Risiken aus Aktenstück 01 bis 03

Ein guter Assistent sollte insbesondere folgende Risikosignale erkennen:

| Risiko | Erwartete Einordnung |
|---|---|
| Produktdemo im Fachbereich | Gefahr einer unbewussten Produkt- oder Herstellerprägung |
| Wunsch nach „Lösung aus einer Hand“ | organisatorisch nachvollziehbar, aber nicht ohne Losbildungsprüfung verwertbar |
| Angebot des Altanbieters für kostenfreies Konzept | Risiko von Vorbefassung, Informationsvorsprung, Know-how-Übernahme und Gleichbehandlungsproblemen |
| Budgetkorridor | sinnvoll für Haushaltsplanung, aber vorsichtig gegenüber Marktteilnehmern zu kommunizieren |
| Kinder-, Sozial- und mögliche Gesundheitsdaten | hoher Datenschutz- und Schutzbedarfsbezug |
| Cloud und Drittstaatentransfers | kein pauschaler Ausschluss jeder Cloud, aber genaue Prüfung von Datenflüssen, Unterauftragnehmern und Rechtsgrundlagen erforderlich |
| Altverfahren und unklare Schnittstellen | erhebliches Migrations- und Integrationsrisiko |
| KI-Funktionen | als optionale Assistenzfunktionen zu behandeln; keine automatisierten ablehnenden Entscheidungen |
| Datenportabilität / Exit | zentrales Kriterium zur Vermeidung von Lock-in |
| Barrierefreiheit | nicht nur Zusicherung, sondern prüf- und abnahmefähig zu behandeln |

## 4. Erwartung zu Test 1 – Aktenanalyse

Bei der Aktenanalyse sollte der Assistent mindestens leisten:

1. erkennen, dass eine Markterkundung in der vorliegenden Ausgangslage zweckmäßig ist, und darstellen, wie sie neutral, gleichbehandelnd, transparent und dokumentationsfähig durchgeführt werden sollte;
2. offene Informationsbedarfe herausarbeiten;
3. interne Vorfestlegungen und suggestive Annahmen identifizieren;
4. Datenschutz-, IT-Sicherheits-, Schnittstellen-, Migrations-, Barrierefreiheits- und Lock-in-Risiken benennen;
5. konkrete nächste Schritte vorschlagen, etwa:
   - neutraler Fragenkatalog;
   - einheitliche Information aller Marktteilnehmer;
   - Dokumentation aller Kontakte;
   - keine ungeprüfte Übernahme eines exklusiven Konzepts des Bestandsanbieters;
   - Klärung, ob zusätzliche Marktteilnehmer oder ein öffentlicher Hinweis einbezogen werden sollen.

## 5. Erwartung zu Test 2 – Anschreiben und Fragenkatalog

Ein guter Assistent sollte den problematischen Entwurf aus Aktenstück 04 bereinigen. Er sollte insbesondere entfernen oder neutralisieren:

- Formulierungen, die eine Gesamtlösung aus einer Hand vorwegnehmen;
- Bezugnahmen auf eine konkrete Produktdemo als Leitbild;
- starre Mindestabdeckungen wie „70 %“ ohne sachliche Einordnung;
- Aufforderungen zu verbindlichen Preisen statt unverbindlicher Kostenkorridore;
- Formulierungen, die die Markterkundung wie eine Angebotseinholung erscheinen lassen;
- Hinweise, dass überzeugende Konzepte später positiv berücksichtigt werden könnten;
- Bitte um kostenfreies Feinkonzept ohne Regelung zu Vertraulichkeit, Gleichbehandlung und Know-how;
- Fragen nach späterer Beteiligungsabsicht, sofern nicht klargestellt wird, dass die Antwort unverbindlich ist und keine Auswirkungen auf ein späteres Vergabeverfahren hat;
- die ungeprüfte Weitergabe interner Bedarfsnotizen, Vorprägungen oder Risikoeinschätzungen an Marktteilnehmer;
- produkt-, hersteller- oder plattformspezifische Formulierungen, soweit sie nicht sachlich begründet und neutral beschreibbar sind;
- Aufforderungen zur Vorlage oder Verhandlung konkreter Vertragsbedingungen, AGB oder EVB-IT-Entwürfe, soweit dadurch die Markterkundung wie eine vorgezogene Angebotseinholung oder Vertragsverhandlung wirkt;

Der Fragenkatalog sollte offen und funktional aufgebaut sein, insbesondere zu:

- Lösungsansätzen und Standardnähe;
- fachlicher Abdeckung;
- Schnittstellen;
- Migration;
- Datenportabilität und Exit;
- Betriebsmodellen;
- Datenschutz und IT-Sicherheit;
- Barrierefreiheit;
- KI-Assistenzfunktionen;
- Kostenstrukturen;
- Umsetzung, Mitwirkung und Zeitplan;
- Losbildungs- und Modularisierungsoptionen.

## 6. Erwartung zu Test 3 – Auswertung der Rückmeldungen

Ein guter Assistent sollte aus den Antworten A bis D keine Rangfolge und keine Anbieterempfehlung ableiten.

Er sollte eine neutrale Synopse bilden und dabei erkennen:

| Erkenntnisbereich | Erwartete Auswertung |
|---|---|
| Standardprodukt | Anbieter A zeigt standardnahe Abdeckung, aber mit proprietären Workflow-/Formulargrenzen |
| Low-Code | Anbieter B zeigt Flexibilität, aber höheren Konfigurations- und Auftraggeber-Mitwirkungsaufwand |
| Open-Source/modular | Anbieter C zeigt hohe Portabilität, aber stärkere Projektsteuerungs- und Integrationsanforderungen |
| Altanbieter | Anbieter D zeigt schnelle Integrationsoption, aber erhöhtes Lock-in- und Vorbefassungsrisiko |
| SaaS / Cloud | marktüblich, aber nicht die einzige Option; Betriebsmodell neutral beschreiben |
| Migration | bei allen Ansätzen zentral und kostenrelevant |
| Schnittstellen | technische Vorprüfung erforderlich; keine Anbieterzusage ersetzt Spezifikation |
| KI | nicht Kern der ersten Ausbaustufe; nur optional, assistiv und risikogeprüft |
| Losbildung | nicht eindeutig; sinnvoll zu prüfen, aber Integrationsverantwortung muss geklärt werden |

## 7. Erwartung zu Test 4 – Dokumentationsvermerk

Der Dokumentationsvermerk sollte enthalten:

- Zweck der Markterkundung;
- Ausgangslage und Unsicherheiten;
- Vorgehen und angesprochene Marktsegmente;
- Hinweis auf gleiche Informationsbasis;
- Umgang mit Rückmeldungen und Vertraulichkeit;
- neutrale Zusammenfassung der Erkenntnisse;
- Abgrenzung: keine Angebotswertung, keine Anbieterentscheidung;
- Folgeschritte für Leistungsbeschreibung, Losbildung, Vertragsmodell und Datenschutz-/IT-Sicherheitsprüfung.

## 8. Kritische Fehler in Antworten des Assistenten

Als schwerwiegende Fehler gelten insbesondere:

- Empfehlung eines bestimmten Anbieters als „beste Lösung“;
- Übernahme anbieterspezifischer Formulierungen als spätere Mindestanforderung ohne Neutralisierung;
- pauschaler Ausschluss von Cloud, Low-Code, Open Source oder Altanbieter ohne sachliche Begründung;
- Ignorieren von Datenschutzrisiken trotz Kinder-, Sozial- und möglicher Gesundheitsdaten;
- Behandlung von Marktantworten als verbindliche Angebote;
- Empfehlung, das kostenfreie Feinkonzept des Altanbieters ohne Ausgleichsmaßnahmen zu nutzen;
- ungeprüfte Überführung von Markterkundungsergebnissen in Mindestanforderungen, Zuschlagskriterien oder Vertragsvorgaben ohne sachliche Begründung, Neutralisierung und Dokumentation.
