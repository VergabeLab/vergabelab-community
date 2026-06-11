---
title: "Testakte M-IT-01 – IT-Ist-Landschaft, Ziele und offene Punkte"
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


# Aktenstück 02 – IT-Ist-Landschaft, Ziele und offene Punkte

## 1. Nutzergruppen

| Nutzergruppe | Geschätzte Zahl | Rolle |
|---|---:|---|
| Sorgeberechtigte / volljährige Schüler:innen | ca. 38.000 potenzielle Nutzer:innen | Antragstellung, Nachweise, Kommunikation |
| Schulen | 52 Schulen | Bestätigung von Schulbesuch, Rückfragen, Statussicht |
| Sachbearbeitung | ca. 90 Mitarbeitende | Prüfung, Kommunikation, Bescheidvorbereitung |
| Teamleitung | 9 Personen | Steuerung, Eskalation, Auswertung |
| Externe Dienstleister | 6 Busunternehmen, 3 Caterer, 1 IT-Dienstleister | Datenabgleich, Abrechnung, Statusmeldungen |
| IT-Administration | 8 Personen | Betrieb, Rechte, Schnittstellen |

## 2. Aktuelle Systeme

| System | Status | Schnittstellenlage |
|---|---|---|
| Dokumentenmanagementsystem `DMS-Nord` | eingeführt, stabil | REST-API vorhanden, aber nur teilweise dokumentiert |
| Fachverfahren `SchulFach 9` | Altverfahren, Wartung bis 2030 | CSV-Import, SOAP-API eingeschränkt |
| Formularserver Landesportal | in Nutzung | XÖV-nahe Datenformate möglich, aber noch nicht produktiv getestet |
| Identity Provider | kommunaler IdP mit SAML/OIDC | BundID-Anbindung in Planung |
| E-Payment | bisher nur Pilot | Schnittstelle noch offen |
| E-Akte | politisch gewünscht | noch keine finale Architekturentscheidung |

## 3. Datenarten

Die Lösung verarbeitet voraussichtlich:

- Stammdaten von Kindern, Sorgeberechtigten und Haushalten;
- Schul- und Klasseninformationen;
- Wohnort- und Beförderungsdaten;
- Nachweise zu Einkommen, Leistungsbezug oder Härtefällen;
- Gesundheitsbezogene Angaben nur in Ausnahmefällen, etwa bei besonderem Beförderungsbedarf;
- Kommunikations- und Statusdaten;
- Protokolldaten und Rollen-/Rechteinformationen.

## 4. Fachliche Ziele

Die AöR möchte:

- digitale Antragstellung mit Upload von Nachweisen;
- medienbrucharme Sachbearbeitung;
- Statusinformationen für Antragstellende;
- standardisierte Rückfragen und Nachforderungen;
- Fristen- und Aufgabensteuerung;
- Bescheidvorbereitung, aber keine vollautomatisierten ablehnenden Entscheidungen;
- Auswertungen für Steuerung und Controlling;
- Mehrmandantenfähigkeit für mehrere Trägerkommunen;
- Nachnutzbarkeit für weitere kommunale Leistungen.

## 5. Nicht-Ziele

Zum jetzigen Zeitpunkt sollen **nicht** beschafft werden:

- vollständiger Ersatz aller Fachverfahren;
- automatisierte Leistungsentscheidung ohne menschliche Prüfung;
- zentrale Bürgerdatenplattform für alle kommunalen Leistungen;
- Lösung ohne dokumentierte Schnittstellen, nachvollziehbare Datenexporte und tragfähige Migrationsmöglichkeit;
- Lösung, die nur mit einem bestimmten DMS oder nur mit einer bestimmten Cloudplattform funktioniert.

## 6. Fachlich-technische Klärungspunkte für die Markterkundung

1. In welchem Umfang können marktverfügbare Standardprodukte die beschriebenen Prozesse abdecken?
2. Welche Anforderungen würden typischerweise eine Individualentwicklung oder erhebliche Anpassungen erfordern?
3. Welche Rolle können Low-Code-Plattformen bei vergleichbaren Vorhaben spielen, und welcher Eigenentwicklungs- oder Betriebsaufwand ist damit verbunden?
4. Welche Betriebsmodelle sind für vergleichbare Portallösungen marktüblich: SaaS, Private Cloud, kommunales Rechenzentrum oder On-Premises?
5. Welche Anforderungen an Datenportabilität, Exportformate und Herausgabe von Konfigurationen sind marktüblich und praktisch erfüllbar?
6. Welche Schnittstellen zu DMS, Identity Provider, Fachverfahren, E-Payment und Formularservern werden regelmäßig unterstützt?
7. Welche Migrationsleistungen sind typischerweise erforderlich, und welche Mitwirkungspflichten entstehen auf Auftraggeberseite?
8. Ob und nach welchen Kriterien lassen sich Leistungen sachgerecht in Lose oder Module aufteilen, etwa Portal/Workflow, Migration/Schnittstellen, Betrieb und Schulung?
9. Welche Barrierefreiheitsstandards werden für vergleichbare Portale üblicherweise erfüllt?
10. Welche KI-gestützten Funktionen werden marktüblich angeboten, und welche davon sind lediglich Assistenzfunktionen ohne automatisierte Entscheidung?


## 7. Vorläufige Risikoeinschätzung der Vergabestelle

| Risiko | Erste Einschätzung |
|---|---|
| Produktzuschnitt | hoch, weil der Fachbereich bereits eine konkrete Produktdemo gesehen hat |
| Datenschutz | hoch, wegen Kindern, Sozialdaten und möglichen Gesundheitsdaten |
| IT-Sicherheit | mittel bis hoch, wegen Portalbetrieb, Identitätsmanagement und externer Zugriffe |
| Schnittstellenrisiko | hoch, wegen Altverfahren und unklarer API-Dokumentation |
| Lock-in | hoch, wenn Prozessmodelle, Formulare, Konfigurationen und Daten nicht exportierbar sind |
| Haushaltsrisiko | mittel, da der Budgetrahmen noch unsicher ist |
| Zeitplanrisiko | hoch, wenn Migration, Schnittstellenklärung und Mitwirkungspflichten unterschätzt werden |
| Vergaberechtliches Risiko | mittel bis hoch, wenn Markterkundungsergebnisse ungeprüft oder anbieterbezogen in spätere Anforderungen einfließen |
