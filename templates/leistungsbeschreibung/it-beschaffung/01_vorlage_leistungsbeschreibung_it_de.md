---
title: "Vorlage – Leistungsbeschreibung IT-Beschaffung"
version: "0.1.0"
last_reviewed: "2026-06-12"
status: "initial"
language: "de-DE"
type: "template"
license: "CC-BY-4.0"
repository_area: "templates/leistungsbeschreibung/it-beschaffung"
module_id: "leistungsbeschreibung-it-beschaffung"
module: "leistungsbeschreibung"
procurement_area: "it-beschaffung"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Vergabepraktiker"
  - "Community-Mitwirkende"
topics:
  - "Leistungsbeschreibung"
  - "IT-Beschaffung"
  - "Template"
  - "VergabeLab Community"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

*VergabeLab Community – Vorlage (Stand: Juni 2026) • © Okan Doğan • Lizenz: CC BY 4.0*

# Vorlage – Leistungsbeschreibung IT-Beschaffung

Diese Vorlage dient als Arbeitsstruktur für Leistungsbeschreibungen im Bereich IT-Beschaffung. Sie ist an den konkreten Beschaffungsgegenstand anzupassen und ersetzt keine fachliche, technische, vergabe- oder datenschutzrechtliche Prüfung. Nicht jeder Abschnitt passt für jede Beschaffung. Abschnitte können gestrichen, ergänzt oder in Anlagen ausgelagert werden.

## Nutzungshinweise

- Platzhalter in eckigen Klammern ausfüllen.
- `MUSS` nur für echte Mindestanforderungen verwenden.
- `KANN` nur für bewertbare Anforderungen verwenden, wenn ein späterer Bewertungsmaßstab vorgesehen oder sinnvoll formulierbar ist.
- Optionale Leistungsbestandteile nicht automatisch als `KANN` behandeln.
- A/AE/B/BE nur verwenden, wenn die Vergabestelle dies ausdrücklich als interne Kennzeichnung benötigt.
- Keine Kriterienmatrix in dieses Template integrieren, sondern bei Bedarf separat führen.
- Vertrags-, Datenschutz-, EVB-IT- und Sicherheitsanlagen getrennt prüfen und führen.

## 1. Zweck des Dokuments

`[Beschreiben, welchen Zweck die Leistungsbeschreibung erfüllt und für welchen Beschaffungsgegenstand sie gilt.]`

## 2. Ausgangssituation und Bedarf

### 2.1 Aktuelle Situation

`[Bestehende Systeme, bisherige Arbeitsweise, Medienbrüche, organisatorische Ausgangslage.]`

### 2.2 Fachlicher Bedarf

`[Welches Problem soll gelöst werden? Welche Ziele verfolgt die Beschaffung?]`

### 2.3 Abgrenzung

`[Was ist ausdrücklich nicht Gegenstand der Grundleistung? Welche Themen werden später, optional oder in gesonderten Anlagen behandelt?]`

## 3. Beschaffungsgegenstand und Leistungsumfang

### 3.1 Gegenstand der Leistung

`[Kurze produkt- und herstellerneutrale Beschreibung der zu beschaffenden IT-Leistung.]`

### 3.2 Grundleistung

| Nr.  | Bestandteil der Grundleistung  | Beschreibung   | Hinweis/Prüfpunkt |
| ---- | ------------------------------ | -------------- | ----------------- |
| G-01 | [z. B. Softwarebereitstellung] | [Beschreibung] | [offen/zu klären] |

### 3.3 Nicht Bestandteil der Grundleistung

| Nr.   | Nicht umfasst                     | Grund/Einordnung                                  | Weiterer Umgang                                             |
| ----- | --------------------------------- | ------------------------------------------------- | ----------------------------------------------------------- |
| NG-01 | [z. B. spätere DMS-Schnittstelle] | [optional/perspektivisch/gesonderte Beauftragung] | [Bedarfsposition/Wahlposition/Abrufoption/gesondert prüfen] |

## 4. Nutzergruppen, Rollen und Mengengerüst

### 4.1 Nutzergruppen

| Nutzergruppe   | Beschreibung   | voraussichtliche Anzahl | Startumfang oder perspektivisch?      |
| -------------- | -------------- | ----------------------: | ------------------------------------- |
| [Nutzergruppe] | [Beschreibung] |                [Anzahl] | [Startumfang/perspektivisch/optional] |

### 4.2 Rollen und Berechtigungen

| Rolle   | Zweck   | Rechte/Handlungen | Datenzugriff | Hinweis/Prüfpunkt |
| ------- | ------- | ----------------- | ------------ | ----------------- |
| [Rolle] | [Zweck] | [Rechte]          | [Umfang]     | [offen/zu klären] |

## 5. Betriebsmodell und technische Rahmenbedingungen

Das Betriebsmodell ist produktneutral zu beschreiben. Eine Festlegung auf On-Premises, SaaS, Hosting, Landesrechenzentrum oder ein bestimmtes Lizenz-/Betriebsmodell erfolgt nur, wenn sachlich begründet.

### 5.1 Betriebsmodell

| Thema          | Anforderung/Angabe                    | Status      |
| -------------- | ------------------------------------- | ----------- |
| Betriebsmodell | [offen/festgelegt/Varianten zulässig] | [Prüfpunkt] |

### 5.2 Technische Umgebung

`[Browser, Endgeräte, Netzwerk, Systemumgebung, Mandanten, Organisationseinheiten, technische Randbedingungen.]`

## 6. Funktionale Anforderungen

Funktionale Anforderungen beschreiben, was die Leistung fachlich können muss. Sie sollten eindeutig, prüfbar und produktneutral formuliert sein.

| ID    | Kategorie         | Anforderung              | Einordnung        | Prüf-/Nachweisidee             | Hinweis     |
| ----- | ----------------- | ------------------------ | ----------------- | ------------------------------ | ----------- |
| F-001 | [z. B. Anmeldung] | [Die Lösung muss/kann …] | [MUSS/KANN/offen] | [Test/Demo/Erläuterung/Export] | [Prüfnotiz] |

`MUSS` nur verwenden, wenn die Anforderung als Mindestanforderung erforderlich und prüfbar ist. `KANN` nur verwenden, wenn sie später qualitativ bewertet werden soll oder sinnvoll bewertbar ist. Unbestimmte Begriffe sind zu konkretisieren oder als Prüfpunkt zu markieren.

## 7. Nichtfunktionale Anforderungen

### 7.1 Benutzbarkeit und Barrierefreiheit

Keine unbestimmten Anforderungen wie `intuitiv`, `benutzerfreundlich` oder `barrierearm` ohne Konkretisierung verwenden. Standards, Prüfmaßstäbe oder Platzhalter ergänzen.

| ID     | Thema            | Anforderung                      | Einordnung   | Konkretisierung/Prüfpunkt                   |
| ------ | ---------------- | -------------------------------- | ------------ | ------------------------------------------- |
| NF-001 | Barrierefreiheit | [konkreter Standard festzulegen] | [MUSS/offen] | [BITV/WCAG/landesrechtliche Vorgabe prüfen] |

### 7.2 Leistung, Verfügbarkeit und Skalierbarkeit

| ID     | Thema       | Anforderung                             | Einordnung        | Mess-/Prüfpunkt           |
| ------ | ----------- | --------------------------------------- | ----------------- | ------------------------- |
| NF-010 | Performance | [Antwortzeit/Last/Nutzerzahl festlegen] | [MUSS/KANN/offen] | [Messverfahren festlegen] |

### 7.3 Datenschutzbezogene Leistungsfunktionen

Nur leistungsbezogene Funktionen aufnehmen. Datenschutzrechtliche Rollen, AVV, TOM-Katalog, Löschkonzept und Datenschutz-Folgenabschätzung gehören regelmäßig in gesonderte Unterlagen.

| ID     | Funktion              | Anforderung               | Einordnung   | Prüfpunkt                                         |
| ------ | --------------------- | ------------------------- | ------------ | ------------------------------------------------- |
| DS-001 | Löschung/Archivierung | [Funktionale Anforderung] | [MUSS/offen] | [Fristen fachlich/datenschutzrechtlich festlegen] |

### 7.4 Informationssicherheit

Keine pauschalen ISO-/BSI-Anforderungen ohne konkreten Leistungsbezug. Sicherheitsanforderungen funktional und prüfbar formulieren.

| ID     | Thema           | Anforderung                      | Einordnung   | Prüfpunkt                   |
| ------ | --------------- | -------------------------------- | ------------ | --------------------------- |
| IS-001 | Verschlüsselung | [Anforderung/Standard festlegen] | [MUSS/offen] | [Standard/Verfahren prüfen] |

## 8. Schnittstellen, Migration und Datenexport

### 8.1 Schnittstellen

| ID    | Zielsystem/Schnittstelle | Zweck   | Status                     | Anforderung/Prüfpunkt                   |
| ----- | ------------------------ | ------- | -------------------------- | --------------------------------------- |
| S-001 | [System]                 | [Zweck] | [MUSS/KANN/optional/offen] | [Format/Protokoll/Verantwortung klären] |

### 8.2 Migration

| ID    | Datenbestand   | Umfang                    | Einordnung                     | Prüfpunkt              |
| ----- | -------------- | ------------------------- | ------------------------------ | ---------------------- |
| M-001 | [Datenbestand] | [Zeitraum/Menge/Qualität] | [Grundleistung/optional/offen] | [Migrationsweg prüfen] |

### 8.3 Datenexport

`[Beschreiben, welche Daten in welchen Formaten exportierbar sein müssen und wofür.]`

## 9. Einführung, Schulung, Dokumentation und Support

### 9.1 Einführung und Projektvorgehen

| Thema      | Anforderung                        | Einordnung   | Hinweis                                   |
| ---------- | ---------------------------------- | ------------ | ----------------------------------------- |
| Einführung | [Einführung, Pilotierung, Rollout] | [MUSS/offen] | [Projektplan ggf. als separates Dokument] |

### 9.2 Schulung

| Zielgruppe   | Schulungsinhalt | Umfang   | Einordnung                     |
| ------------ | --------------- | -------- | ------------------------------ |
| [Zielgruppe] | [Inhalt]        | [Umfang] | [Grundleistung/optional/offen] |

### 9.3 Dokumentation

`[Benutzer-, Admin-, Schnittstellen-, Betriebs- oder Migrationsdokumentation beschreiben.]`

### 9.4 Support und Wartung

Konkrete Servicezeiten, Reaktionszeiten, Wiederherstellungszeiten, Sanktionen und SLA-Rechtsfolgen sind regelmäßig mit Vertragsunterlagen abzugleichen. In der Leistungsbeschreibung nur fachlich benötigte Supportleistungen beschreiben.

| Thema   | Leistungsanforderung       | Einordnung   | Vertrags-/SLA-Bezug?  |
| ------- | -------------------------- | ------------ | --------------------- |
| Support | [fachlicher Supportbedarf] | [MUSS/offen] | [ggf. Vertragsanlage] |

## 10. Optionale Leistungsbestandteile

Optionale Leistungsbestandteile sind nicht automatisch `KANN`-Anforderungen und nicht automatisch Bewertungskriterien. Zu klären ist, ob sie bepreist, mit angeboten, später abgerufen oder in die Wertung einbezogen werden sollen.

| ID    | Optionaler Leistungsbestandteil | Beschreibung   | Mögliche Einordnung                                            | Klärungsbedarf                      |
| ----- | ------------------------------- | -------------- | -------------------------------------------------------------- | ----------------------------------- |
| O-001 | [z. B. zusätzliches Modul]      | [Beschreibung] | [Bedarfsposition/Wahlposition/Abrufoption/spätere Ausbaustufe] | [Preis/Abruf/Wertung/Umfang klären] |

## 11. Offene Punkte und Prüfnotizen

| Nr.   | Thema   | Offener Punkt/Risiko | Empfohlene Klärung |
| ----- | ------- | -------------------- | ------------------ |
| P-001 | [Thema] | [Risiko]             | [Klärung]          |

## 12. Abgrenzung zu gesonderten Unterlagen

| Thema            | Gehört regelmäßig nicht unmittelbar in die Leistungsbeschreibung | Hinweis                                 |
| ---------------- | ---------------------------------------------------------------- | --------------------------------------- |
| Kriterienkatalog | Punkte, Gewichtungen, Bewertungsmethodik                         | separat führen                          |
| Vertrag/EVB-IT   | Kündigung, Sanktionen, weitere rechtliche Folgen                  | Vertragsunterlagen                      |
| Datenschutz      | AVV, TOM-Katalog, DSFA, Löschkonzept                             | Datenschutzunterlagen                   |
| IT-Sicherheit    | vollständiges Sicherheitskonzept                                 | gesonderte Anlage/Prüfung               |
| Eignung          | Referenzen, Umsatz, Zertifizierungen des Bieters                 | Eignungsanforderungen/Vergabeunterlagen |

## 13. Glossar

| Begriff                         | Erläuterung                                                                                                        |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Mindestanforderung (MUSS)       | zwingend zu erfüllende Anforderung; Nichterfüllung kann zum Ausschluss führen                                      |
| Bewertbare Anforderung (KANN)   | qualitative Anforderung, die nicht zwingend erfüllt sein muss und nur bei Bewertungsabsicht in die Wertung eingeht |
| Optionaler Leistungsbestandteil | zusätzlicher oder späterer Leistungsbestandteil, z. B. Bedarfsposition, Wahlposition, Abrufoption oder Ausbaustufe |
