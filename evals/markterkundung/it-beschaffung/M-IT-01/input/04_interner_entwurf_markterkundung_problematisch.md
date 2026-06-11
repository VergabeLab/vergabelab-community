---
title: "Testakte M-IT-01 – Interner Entwurf Markterkundung, problematische Fassung"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "problematic-draft"
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


# Aktenstück 04 – Interner Entwurf Markterkundung, problematische Fassung

## 1. Einordnung des Dokuments

Dieses Aktenstück enthält einen internen Arbeitsentwurf aus Fachbereich und IT-Abteilung. Einzelne Stellen haben hierzu bereits erste Hinweise oder Randnotizen eingebracht. Der Entwurf ist jedoch **noch nicht** abschließend durch die Vergabestelle, die Datenschutzbeauftragte oder die IT-Sicherheitskoordination geprüft oder freigegeben.

Der Entwurf soll zeigen, welche Formulierungen innerhalb der Verwaltung bereits diskutiert werden. Er ist nicht als Muster zu verstehen.

## 2. Entwurf eines Anschreibens an Marktteilnehmer

**Betreff:** Markterkundung zum Vorhaben `SchulServicePortal`

Sehr geehrte Damen und Herren,

der Kommunale Dienstleistungsverbund Nordtal AöR plant die Einführung eines digitalen Antrags- und Vorgangsportals für schulbezogene Verwaltungsleistungen.

Nach ersten internen Überlegungen benötigen wir eine **Gesamtlösung aus einer Hand**, die möglichst schnell eingeführt werden kann und sich eng an marktgängigen Fachportalen orientiert. Im Fachbereich wurde bereits eine Produktpräsentation gesehen, die aus unserer Sicht viele Anforderungen sehr gut abbildet. Wir möchten daher prüfen, welche Anbieter vergleichbare Lösungen anbieten können.

Wir bitten um Rückmeldung, ob Ihr Unternehmen ein fertiges oder weitgehend fertiges Produkt bereitstellen kann, das insbesondere folgende Punkte erfüllt:

- digitale Antragstellung für Sorgeberechtigte und volljährige Schüler:innen;
- Bearbeitungsworkflow für Sachbearbeitung und Teamleitungen;
- Anbindung an das vorhandene Dokumentenmanagementsystem `DMS-Nord`;
- Anbindung an das Fachverfahren `SchulFach 9`;
- Mehrmandantenfähigkeit für mehrere Trägerkommunen;
- Betrieb als SaaS-Lösung in einer EU-Cloud;
- Einführung bis spätestens T+12 Monate nach Zuschlag;
- optionale KI-Funktionen für Dokumentenerkennung, Textvorschläge und Bürgerkommunikation.

Bitte stellen Sie uns möglichst konkret dar, wie Ihr Produkt diese Anforderungen erfüllt. Idealerweise senden Sie uns bereits eine **Konzeptskizze mit Lösungsarchitektur, Einführungsplan, Lizenzmodell und belastbarer Preisindikation**.

Da die Mittelanmeldung nach T+12 Wochen vorbereitet werden soll, bitten wir zudem um eine möglichst verbindliche Kostenschätzung für Einführung, Migration, Schulung und Betrieb über vier Jahre. Der aktuelle interne Budgetrahmen liegt bei 850.000 EUR bis 1.400.000 EUR netto.

Die Rückmeldungen aus der Markterkundung sollen in die späteren Vergabeunterlagen einfließen. Anbieter, die im Rahmen der Markterkundung besonders überzeugende Konzepte einreichen, können dadurch für die spätere Beschaffung besser eingeordnet werden.

Wir weisen darauf hin, dass die Teilnahme an der Markterkundung nicht vergütet wird. Gleichwohl bitten wir um möglichst detaillierte Unterlagen, damit wir eine belastbare Grundlage für die spätere Ausschreibung erhalten.

Mit freundlichen Grüßen  
Kommunaler Dienstleistungsverbund Nordtal AöR  
Projektgruppe `SchulServicePortal`

## 3. Entwurf eines Fragenkatalogs

1. Verfügen Sie über ein fertiges Produkt, das die Anforderungen des `SchulServicePortal` im Wesentlichen bereits erfüllt?
2. Können Sie bestätigen, dass Ihre Lösung mindestens 70 % der in unserer internen Bedarfsnotiz beschriebenen Prozesse standardmäßig abdeckt?
3. Können Sie die Lösung als Gesamtsystem aus einer Hand liefern, einschließlich Einführung, Migration, Schnittstellen, Betrieb, Schulung und Support?
4. Ist Ihre Lösung mit `DMS-Nord` und `SchulFach 9` kompatibel?
5. Können Sie einen SaaS-Betrieb in einer EU-Cloud sicherstellen?
6. Können Sie ausschließen, dass personenbezogene Daten in Drittstaaten verarbeitet werden?
7. Können Sie spätestens T+12 Monate nach Zuschlag produktiv gehen?
8. Welche KI-Funktionen bieten Sie bereits produktiv an?
9. Können Sie uns eine belastbare Preisindikation innerhalb des genannten Budgetrahmens geben?
10. Halten Sie eine Losbildung für sinnvoll oder sollte aus Ihrer Sicht alles an einen Anbieter vergeben werden?
11. Wären Sie bereit, vorab ein kostenfreies Feinkonzept zu erstellen?
12. Wären Sie bereit, Ihre Produktpräsentation dem Fachbereich kurzfristig vorzustellen?
13. Werden Sie sich voraussichtlich an einem späteren Vergabeverfahren beteiligen?

## 4. Interne Randnotizen zum Entwurf

- Fachbereich: Eine Lösung aus einer Hand wäre organisatorisch am einfachsten.
- IT-Abteilung: Offene Schnittstellen, Datenexporte und Exit-Szenarien müssen zwingend geklärt werden.
- Datenschutzbeauftragte: Kinderdaten, Sozialdaten und mögliche Gesundheitsdaten machen eine sehr genaue Prüfung des Betriebsmodells erforderlich.
- Kämmerei: Für die Haushaltsanmeldung werden belastbare Kostenkorridore benötigt; ein einzelner Anbieterpreis reicht dafür nicht.
- Vergabestelle: Es ist zu prüfen, ob einzelne Formulierungen bereits zu stark auf bestimmte Anbieter, Produkte, Technologien oder Betriebsmodelle hinauslaufen. Zudem ist zu klären, welche internen Informationen überhaupt an Marktteilnehmer herausgegeben werden dürfen und ob hierfür eine bereinigte, neutrale Projektbeschreibung erstellt werden muss.
