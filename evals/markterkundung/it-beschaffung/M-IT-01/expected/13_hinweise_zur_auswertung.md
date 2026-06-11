---
title: "Testakte M-IT-01 – Hinweise zur Auswertung"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "evaluation-guide"
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

*VergabeLab Community – KI-Baustein (Stand: Juni 2026) • © Okan Doğan • Lizenz: CC BY 4.0*

# Aktenstück 13 – Hinweise zur Auswertung

## 1. Zweck dieses Dokuments

Dieses Dokument unterstützt die manuelle Auswertung von Testläufen mit der [Testakte M-IT-01](/evals/markterkundung/it-beschaffung/M-IT-01/). Es richtet sich an Personen, die Antworten von ChatGPT Custom GPTs, Claude Skills oder anderen LLM-Assistenten vergleichen möchten.

Es darf bei Blindtests nicht als Input in den zu testenden Assistenten geladen werden.

## 2. Empfohlene Testdurchführung

### Testmodus A – Vorbereitung der Markterkundung

**Input:** [Aktenstücke 01–05](/evals/markterkundung/it-beschaffung/M-IT-01/input/)
**Geeignete Prompts:** [Test 1](/evals/markterkundung/it-beschaffung/M-IT-01/prompts/01_testprompt_vorbereitung_markterkundung_de.md) und [Test 2](/evals/markterkundung/it-beschaffung/M-IT-01/prompts/02_testprompt_anschreiben_fragenkatalog_de.md) aus der [README](/evals/markterkundung/it-beschaffung/M-IT-01/README.md#empfohlene-test-prompts)

Ziel ist zu prüfen, ob der Assistent aus der Ausgangslage und dem problematischen Entwurf eine neutrale Markterkundung entwickeln kann.

Nicht als Input verwenden:

* [Aktenstücke 06–09](/evals/markterkundung/it-beschaffung/M-IT-01/input/), weil sie bereits Marktrückläufe enthalten;
* [Aktenstücke 10–13](/evals/markterkundung/it-beschaffung/M-IT-01/expected/), weil sie Erwartungshorizont und Scoring enthalten.

### Testmodus B – Auswertung der Marktrückläufe

**Input:** [Aktenstücke 01–09](/evals/markterkundung/it-beschaffung/M-IT-01/input/)
**Geeignete Prompts:** [Test 3](/evals/markterkundung/it-beschaffung/M-IT-01/prompts/03_testprompt_auswertung_marktruecklaeufe_de.md) und [Test 4](/evals/markterkundung/it-beschaffung/M-IT-01/prompts/04_testprompt_dokumentationsvermerk_de.md) aus der [README](/evals/markterkundung/it-beschaffung/M-IT-01/README.md#empfohlene-test-prompts)

Ziel ist zu prüfen, ob der Assistent Anbieterantworten neutral auswertet, ohne eine Rangfolge oder Anbieterempfehlung zu bilden.

Nicht als Input verwenden:

* [Aktenstücke 10–13](/evals/markterkundung/it-beschaffung/M-IT-01/expected/).

### Testmodus C – Regressionstest / Vergleich mehrerer Assistenten

**Input:** je nach Testziel [01–05 oder 01–09](/evals/markterkundung/it-beschaffung/M-IT-01/input/)
**Auswertung:** [Aktenstücke 10–13](/evals/markterkundung/it-beschaffung/M-IT-01/expected/)

Ziel ist, Antworten unterschiedlicher Systeme nach denselben Kriterien zu vergleichen.

## 3. Besondere Hinweise für Custom GPTs

Bei Custom GPTs sollten die [Dateien 10–13](/evals/markterkundung/it-beschaffung/M-IT-01/expected/) nicht als Knowledge-Dateien hochgeladen werden, wenn ein echter Blindtest durchgeführt werden soll.

Empfohlenes Vorgehen:

1. Custom GPT mit dem regulären [Markterkundungs-Systemprompt](/prompts/markterkundung/it-beschaffung/01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md) konfigurieren.
2. Nur die benötigten [Input-Aktenstücke](/evals/markterkundung/it-beschaffung/M-IT-01/input/) als Testmaterial bereitstellen.
3. Einen der [Testprompts](/evals/markterkundung/it-beschaffung/M-IT-01/prompts/) aus der [README](/evals/markterkundung/it-beschaffung/M-IT-01/README.md#empfohlene-test-prompts) verwenden.
4. Antwort speichern.
5. Antwort manuell anhand von [Aktenstück 10 bis 13](/evals/markterkundung/it-beschaffung/M-IT-01/expected/) auswerten.

## 4. Besondere Hinweise für Claude Skills

Bei Claude Skills sollte die [Testakte](/evals/markterkundung/it-beschaffung/M-IT-01/) als Eval-Material getrennt vom Skill selbst gehalten werden. Der Skill darf nicht auf den [Erwartungshorizont](/evals/markterkundung/it-beschaffung/M-IT-01/expected/10_erwartungshorizont_evaluation.md), das [Goldstandard-Outputschema](/evals/markterkundung/it-beschaffung/M-IT-01/expected/11_goldstandard_outputschema.md) oder die [Scoring Rubric](/evals/markterkundung/it-beschaffung/M-IT-01/expected/12_scoring_rubric.md) zugreifen, wenn die Leistungsfähigkeit blind getestet werden soll.

## 5. Ergebnisdokumentation

Testergebnisse können im Ordner [`results/`](/evals/markterkundung/it-beschaffung/M-IT-01/results/) dokumentiert werden. Empfohlenes Namensschema:

```text
results/
  lauf-001_custom-gpt_markterkundung_v0-1_test-1.md
  lauf-002_claude-skill_markterkundung_v0-1_test-1.md
```

Ein Ergebnisvermerk sollte mindestens enthalten:

* getestetes System;
* verwendete Version des Prompts oder Skills;
* verwendete Aktenstücke;
* verwendeter Testprompt;
* Datum des Testlaufs oder relative Einordnung des Testlaufs;
* unveränderte Antwort des Assistenten;
* Bewertung anhand der [Scoring Rubric](/evals/markterkundung/it-beschaffung/M-IT-01/expected/12_scoring_rubric.md);
* kurze qualitative Auswertung.

## 6. Umgang mit Abweichungen

Ein Assistent muss nicht exakt die Formulierungen aus dem [Goldstandard](/evals/markterkundung/it-beschaffung/M-IT-01/expected/11_goldstandard_outputschema.md) verwenden. Gute Antworten können anders strukturiert sein.

Entscheidend ist, ob sie:

* die vergaberechtliche Funktion der Markterkundung zutreffend erfassen;
* problematische Vorfestlegungen erkennen;
* neutral und diskriminierungsfrei formulieren;
* Datenschutz-, IT-Sicherheits-, Schnittstellen-, Migrations- und Lock-in-Risiken berücksichtigen;
* Rückmeldungen von Marktteilnehmern nicht als Angebotswertung behandeln;
* Ergebnisse dokumentationsfähig aufbereiten.

## 7. Typische Schwächen bei Testläufen

Bei der Auswertung sollte besonders auf folgende Schwächen geachtet werden:

* zu frühe Empfehlung eines konkreten Lösungsansatzes;
* unkritische Übernahme von Anbieterangaben;
* fehlende Trennung zwischen Marktinformation und Vergabeanforderung;
* zu allgemeiner Fragenkatalog ohne Bezug zu Daten, Schnittstellen, Migration und Exit;
* fehlender Umgang mit dem Altanbieter und dem informellen Konzeptangebot;
* fehlende Hinweise zu Barrierefreiheit und KI-Funktionen;
* fehlende Dokumentationsstruktur für die Vergabeakte.

## 8. Pflege der Testakte

Wenn die [Input-Aktenstücke 01–09](/evals/markterkundung/it-beschaffung/M-IT-01/input/) geändert werden, sollten auch [Erwartungshorizont](/evals/markterkundung/it-beschaffung/M-IT-01/expected/10_erwartungshorizont_evaluation.md), [Goldstandard-Outputschema](/evals/markterkundung/it-beschaffung/M-IT-01/expected/11_goldstandard_outputschema.md) und [Scoring Rubric](/evals/markterkundung/it-beschaffung/M-IT-01/expected/12_scoring_rubric.md) geprüft werden. Andernfalls besteht die Gefahr, dass die Bewertung nicht mehr zur Testakte passt.

Änderungen sollten versioniert und in der [README](/evals/markterkundung/it-beschaffung/M-IT-01/README.md) nachvollziehbar dokumentiert werden.
