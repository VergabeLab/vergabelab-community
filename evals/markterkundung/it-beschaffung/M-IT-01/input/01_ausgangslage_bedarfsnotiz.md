---
title: "Testakte M-IT-01 – Ausgangslage und Bedarfsnotiz"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "case-context"
eval_role: "input"
eval_case_id: "M-IT-01"
relative_date: "T0"
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


# Aktenstück 01 – Ausgangslage und Bedarfsnotiz

## 1. Fiktiver Auftraggeber

**Kommunaler Dienstleistungsverbund Nordtal AöR**  
Fiktive Anstalt öffentlichen Rechts, gebildet von mehreren kreisangehörigen Kommunen. Keine echte Körperschaft.

## 2. Arbeitstitel des Vorhabens

**Digitales Antrags- und Vorgangsportal für schulbezogene Verwaltungsleistungen**

Interner Arbeitstitel: `SchulServicePortal`

## 3. Ausgangslage

Der Kommunale Dienstleistungsverbund Nordtal AöR bündelt für seine Trägerkommunen sowie für angeschlossene kommunale Schulträger und Aufgabenträger bestimmte schulbezogene Verwaltungs- und Unterstützungsleistungen. Die Aufgabenwahrnehmung beruht fiktiv auf einer landesrechtlich zulässigen Form interkommunaler Zusammenarbeit, insbesondere auf Satzung, öffentlich-rechtlicher Vereinbarung oder Aufgabenübertragung. Die AöR nimmt keine schulaufsichtlichen oder pädagogischen Aufgaben wahr.

Zum Aktenstand werden Anträge überwiegend per PDF, E-Mail und Papier eingereicht. Die Bearbeitung erfolgt in mehreren Fachbereichen mit Medienbrüchen.

Betroffene Leistungen, soweit sie im Zuständigkeitsbereich der angeschlossenen Träger liegen:

* Schülerbeförderung und Erstattung von Fahrtkosten;
* Anträge auf Lernmittelfreiheit oder vergleichbare Lernmittelunterstützung;
* Zuschüsse für Mittagsverpflegung;
* Ausgabe und Rücknahme kommunaler Leihgeräte;
* Härtefallanträge und Einzelfallprüfungen;
* Kommunikation mit Schulen, Sorgeberechtigten und externen Dienstleistern.

Die AöR möchte prüfen, ob der Markt standardisierte oder weitgehend standardnahe Lösungen anbietet, die diese Prozesse digital, datenschutzkonform und wirtschaftlich abbilden können.

## 4. Anlass der Markterkundung

Die Fachabteilung hat zunächst angenommen, dass eine Individualentwicklung erforderlich ist. Die IT-Abteilung hält dagegen ein Standardprodukt oder eine Low-Code-Plattform für möglich. Die Kämmerei möchte vor einer Haushaltsanmeldung belastbare Größenordnungen und Betriebsmodelle kennen. Die Vergabestelle möchte vermeiden, dass die spätere Leistungsbeschreibung auf eine einzelne technische Lösung oder einen bekannten Anbieter zugeschnitten wird.

Die Markterkundung soll daher klären:

- Welche Lösungsansätze am Markt bestehen: Fachportal, Low-Code-Plattform, DMS-/Workflow-Erweiterung, Individualentwicklung, Open-Source-Ansatz, SaaS, Private Cloud, On-Premises;
- welche Mindestinformationen für eine funktionale Leistungsbeschreibung fehlen;
- welche Schnittstellen, Migrationen und Betriebsmodelle realistisch sind;
- welche Kosten- und Lizenzmodelle marktüblich sind;
- welche Risiken aus Datenschutz, IT-Sicherheit, Barrierefreiheit, KI-Funktionen und Anbieterbindung folgen;
- welche fachlichen, technischen und betrieblichen/wirtschaftlichen Erkenntnisse für die spätere Prüfung der Losbildung erforderlich sind, insbesondere zur Abgrenzung möglicher Fach- oder Teillose und zur Begründung einer etwaigen Gesamtvergabe.

## 5. Grober Zeitplan

| Meilenstein | Interner Zielzeitpunkt |
|---|---:|
| Eingang der initialen Bedarfsmeldung einschließlich Bedarfserhebungsbogen | T0 |
| Interne Sichtung durch Vergabestelle | T+1 Woche |
| Abstimmung mit IT, Datenschutz und Kämmerei | T+2 Wochen |
| Markterkundung vorbereiten | T+3 Wochen |
| Markterkundung durchführen | T+4 bis T+8 Wochen |
| Auswertung der Markterkundung | T+10 Wochen |
| Entscheidung über Beschaffungsstrategie und Mittelanmeldung | T+12 Wochen |
| Start des Vergabeverfahrens | frühestens T+20 Wochen |
| Zuschlag | frühestens T+36 Wochen |
| Produktivstart Pilotkommune | frühestens T+12 Monate |
| Rollout auf alle Trägerkommunen | frühestens T+18 Monate |

## 6. Budgetrahmen

Für die Haushaltsplanung steht ein vorläufiger Korridor von **850.000 EUR bis 1.400.000 EUR netto** für Einführung, Migration, Schulung und Betrieb über vier Jahre im Raum. Der Korridor ist unsicher und soll durch die Markterkundung plausibilisiert werden. Er darf gegenüber Marktteilnehmern nur so kommuniziert werden, dass keine Preissteuerung ausgelöst wird.

## 7. Vorläufige rechtliche Einordnung

Die Vergabestelle geht zum Aktenstand von einem EU-weiten Vergabeverfahren oberhalb des maßgeblichen Schwellenwerts aus. Die konkrete Verfahrensart ist noch offen. Diskutiert werden insbesondere:

* offenes Verfahren mit funktionaler Leistungsbeschreibung;
* nichtoffenes Verfahren mit Teilnahmewettbewerb;
* Verhandlungsverfahren mit Teilnahmewettbewerb, falls der Leistungsgegenstand ohne vorherige Verhandlungen nicht hinreichend bestimmt werden kann.

Unabhängig von der Verfahrensart soll geprüft werden, ob eine Losbildung nach fachlichen, technischen oder betrieblichen Modulen sachlich sinnvoll und vergaberechtlich geboten ist.

## 8. Interne Spannungen

- Der Fachbereich bevorzugt „eine Lösung aus einer Hand“.
- Die IT-Abteilung möchte keine neue isolierte Fachanwendung ohne offene Schnittstellen.
- Die Datenschutzbeauftragte warnt vor Cloud-Lösungen mit Drittstaatentransfers.
- Die Kämmerei drängt auf belastbare Zahlen vor dem Haushaltsbeschluss.
- Ein Altanbieter hat informell angeboten, „kostenlos ein Konzept zu schreiben“, wenn er später in das Verfahren einbezogen wird.
- Eine Produktpräsentation eines bekannten Herstellers hat den Fachbereich stark beeinflusst.

## 9. Offene Prüffragen zum Vorgehen

Vor einer Entscheidung über das weitere Vorgehen möchte die Vergabestelle klären, welche Erkenntnisse durch eine Markterkundung gewonnen werden sollen und wie sie ausgestaltet werden muss, damit die bestehenden fachlichen, technischen und wirtschaftlichen Unsicherheiten neutral, vergleichbar und dokumentationsfähig aufgearbeitet werden können.

Aus Sicht der Vergabestelle sind insbesondere folgende Punkte offen:

* Welche Informationen fehlen, um den Bedarf später funktional und neutral beschreiben zu können?
* Welche internen Annahmen könnten bereits zu stark auf bestimmte Lösungen, Produkte, Anbieter oder Betriebsmodelle hinauslaufen?
* Welche Marktinformationen können zulässig abgefragt werden, ohne eine spätere Anbieterwertung oder Beschaffungsentscheidung vorwegzunehmen?
* Welche Erkenntnisse werden benötigt, um mögliche Fach- oder Teillose zu prüfen und eine etwaige Gesamtvergabe tragfähig begründen zu können?
* Wie sollte die Markterkundung dokumentiert werden, damit ihre Ergebnisse später nachvollziehbar, transparent und diskriminierungsfrei in die weitere Beschaffung einfließen können?
