---
title: "Testakte M-IT-01 – Goldstandard Outputschema"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "goldstandard-outputschema"
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


# Aktenstück 11 – Goldstandard Outputschema

## 1. Zweck dieses Dokuments

Dieses Aktenstück beschreibt ein ideales Outputschema für die Antworten eines Assistenten. Es dient der internen Evaluation und darf bei Blindtests nicht als Input in den zu testenden Assistenten geladen werden.

Das Schema ist nicht als starre Musterlösung zu verstehen. Ein Assistent kann gleichwertige Ergebnisse auch anders strukturieren, solange die fachlichen Kernleistungen erreicht werden.

## 2. Goldstandard-Schema für Test 1 – Aktenanalyse

### Aktenanalyse zur geplanten Markterkundung

#### 1. Kurzbefund

Die Markterkundung ist zweckmäßig, weil der Bedarf erkennbar, aber der Lösungsraum noch offen ist. Sie muss neutral, dokumentiert und ohne Anbieter- oder Produktvorfestlegung durchgeführt werden.

#### 2. Noch fehlende Informationen

- fachliche Priorisierung der Leistungen;
- Soll-Prozesse und Varianten je Trägerkommune;
- Datenflüsse und Rollenmodell;
- Schnittstellendokumentation zu DMS, Fachverfahren, IdP, Formularserver und E-Payment;
- Migrationsumfang und Datenqualität;
- Betriebs- und Supportanforderungen;
- Barrierefreiheits- und Sicherheitsanforderungen;
- Umgang mit KI-Funktionen;
- Anforderungen an Datenportabilität und Exit.

#### 3. Risikobewertung

| Risiko | Einordnung | Empfohlene Maßnahme |
|---|---|---|
| Produktzuschnitt | hoch | Fragen funktional formulieren, keine Produktdemo als Leitbild |
| Altanbieter / Konzeptangebot | hoch | keine Exklusivität, gleiche Informationen, Vorbefassung dokumentieren |
| Datenschutz | hoch | Datenarten, Rollen, AVV, DSFA-Prüfung, Löschkonzept abfragen |
| Schnittstellen | hoch | Schnittstellenmatrix und technische Vorprüfung verlangen |
| Lock-in | hoch | Exportformate, Exit, Dokumentation und Rechte abfragen |
| KI | mittel bis hoch | nur optional, assistiv, keine automatisierten Ablehnungen |
| Budget | mittel | nur Kostenkorridore abfragen, keine Preissteuerung |

#### 4. Nächste Schritte

1. problematischen Entwurf bereinigen;
2. einheitlichen Fragenkatalog erstellen;
3. identische Informationsbasis an alle Marktteilnehmer geben;
4. Rückmeldungen in Synopse auswerten;
5. Ergebnisse neutral in Leistungsbeschreibung, Losbildungsprüfung und Vertragsstrategie überführen.

## 3. Goldstandard-Schema für Test 2 – Anschreiben und Fragenkatalog

### Neutrales Markterkundungsanschreiben
```markdown
Sehr geehrte Damen und Herren,

der Kommunale Dienstleistungsverbund Nordtal AöR prüft die Vorbereitung einer möglichen Beschaffung für ein digitales Antrags- und Vorgangsportal für schulbezogene Verwaltungsleistungen.

Ziel dieser Markterkundung ist es, einen Überblick über marktgängige Lösungsansätze, Betriebsmodelle, Schnittstellen, Migrationsaufwände, Kostenstrukturen und Risiken zu gewinnen. Die Markterkundung ist keine Aufforderung zur Angebotsabgabe und keine Vorentscheidung über ein späteres Vergabeverfahren.

Alle Rückmeldungen werden ausschließlich zur Vorbereitung einer neutralen und diskriminierungsfreien Leistungsbeschreibung sowie zur internen Planung ausgewertet. Aus der Teilnahme oder Nichtteilnahme entstehen keine Vor- oder Nachteile für ein etwaiges späteres Vergabeverfahren.

[...]
```

### Fragenkatalog

#### A. Lösungsansatz und Standardnähe

1. Welche Lösungsansätze kommen aus Ihrer Sicht für den beschriebenen Bedarf in Betracht?
2. Welche Bestandteile können standardnah abgebildet werden?
3. Welche Bestandteile erfordern typischerweise Anpassung, Konfiguration oder Individualentwicklung?

#### B. Fachliche Abdeckung

[Fragen zu Antragstellung, Workflow, Status, Nachweisen, Bescheidvorbereitung, Mehrmandantenfähigkeit]

#### C. Schnittstellen und Integration

[Fragen zu DMS, Fachverfahren, IdP, Formularserver, E-Payment, APIs, Datenformaten]

#### D. Migration und Mitwirkung

[Fragen zu Datenqualität, Migrationsphasen, Testmigration, Mitwirkungspflichten]

#### E. Betrieb, Datenschutz und IT-Sicherheit

[Fragen zu Betriebsmodellen, AVV, Mandantentrennung, Protokollierung, Löschung, Schutzbedarf]

#### F. Datenportabilität und Exit

[Fragen zu Exportformaten, Dokumentation, Herausgabe von Konfigurationen, Exit-Unterstützung]

#### G. Barrierefreiheit

[Fragen zu Standards, Nachweisen, Tests, redaktionellen Pflichten]

#### H. KI-Assistenzfunktionen

[Fragen zu optionalen Funktionen, Datenverarbeitung, menschlicher Kontrolle, Deaktivierbarkeit]

#### I. Kostenstrukturen und Umsetzung

[Fragen zu unverbindlichen Kostenkorridoren, Kostentreibern, Zeitplan, Schulung, Support]

#### J. Losbildung und Modularisierung

[Fragen zu fachlich oder technisch trennbaren Leistungsbestandteilen und Integrationsverantwortung]


## 4. Goldstandard-Schema für Test 3 – Auswertung der Marktrückläufe

### Synopse der Marktrückläufe

| Thema | Anbieter A | Anbieter B | Anbieter C | Anbieter D | Auswertung |
|---|---|---|---|---|---|
| Lösungsansatz | Standardportal | Low-Code | modular/open-source-nah | Erweiterung Altverfahren | mehrere marktgängige Ansätze, keine zwingende Einzellösung |
| Standardnähe | mittel bis hoch | abhängig von Konfiguration | gering, eher Projektansatz | hoch bei Fortführung Altverfahren | funktionale Beschreibung erforderlich |
| Schnittstellen | REST/OIDC/CSV/XML | REST/OIDC/Adapter | offene Integrationsschicht | proprietär geprägt | Schnittstellenmatrix erforderlich |
| Datenportabilität | teilweise offen | plattformeigenes JSON | stark | eingeschränkt | Exit-Anforderungen wichtig |
| Betrieb | SaaS EU, optional anders | mehrere Modelle | kommunales RZ/Private Cloud | bestehendes Umfeld/Hosting | Betriebsmodell neutral beschreiben |
| KI | optional assistiv | optional, eher später | zunächst nicht empfohlen | Roadmap unklar | nicht als Kernanforderung |
| Lock-in | mittel | mittel | niedrig bis mittel | hoch | Lock-in differenziert adressieren |


## 5. Goldstandard-Schema für Test 4 – Dokumentationsvermerk

### Dokumentationsvermerk Markterkundung

#### 1. Zweck

Die Markterkundung diente der Vorbereitung einer möglichen IT-Beschaffung und der Klärung des noch offenen Lösungsraums. Sie war nicht auf die Auswahl eines Anbieters oder die Vorwegnahme einer Zuschlagsentscheidung gerichtet.

#### 2. Vorgehen

[einheitliche Ansprache, gleiche Informationsbasis, vier Marktsegmente, Rückmeldefrist, Dokumentation]

#### 3. Wesentliche Erkenntnisse

[mehrere Lösungsansätze, Schnittstellen und Migration zentral, Cloud möglich aber prüfbedürftig, KI nur optional, Datenportabilität/Exit wichtig]

#### 4. Vergaberechtliche Einordnung

[keine Angebotswertung, keine Rangfolge, Neutralisierung von Anbieterinformationen, Prüfung Losbildung]

#### 5. Folgeschritte

[Bedarfspräzisierung, Schnittstellenanalyse, Datenschutz-/IT-Sicherheitsprüfung, Losbildungsprüfung, Vertrags- und Betriebsmodell]

#### 6. Erwartete Tonalität

Die Antwort sollte sachlich, vergaberechtlich präzise und praktisch verwertbar sein. Sie sollte keine werbenden Formulierungen, keine Anbieterpräferenz und keine spekulativen rechtlichen Gewissheiten enthalten.
