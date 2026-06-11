---
title: "Modulstruktur in der VergabeLab Community"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "guide"
license: "CC-BY-4.0"
repository_area: "guides"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Community-Mitwirkende"
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Entwicklerinnen und Entwickler"
topics:
  - "Modulstruktur"
  - "Metadaten"
  - "module_id"
  - "Evaluation"
  - "VergabeLab Community"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# Modulstruktur in der VergabeLab Community

## 1. Warum Module?

Viele Bausteine in der VergabeLab Community sind fachlich aufeinander bezogen. Ein Prompt allein reicht regelmäßig nicht aus, um eine Aufgabe verlässlich, prüfbar und wiederverwendbar zu unterstützen.

Qualität entsteht durch das Zusammenspiel von steuernden Hinweisen, fachlichem Wissen, wiederverwendbaren Vorlagen und geeigneten Evaluationsmaterialien. Die Modulstruktur hilft dabei, solche zusammengehörigen Bausteine nachvollziehbar zu ordnen.

## 2. Was gehört zu einem Modul?

Ein Modul beschreibt einen fachlich zusammenhängenden Arbeitsbereich im Repository. Es kann typischerweise Bausteine aus mehreren Bereichen enthalten:

- `prompts/`: Prompt- und Hinweistexte für KI-gestützte Assistenzsysteme.
- `wissen/`: fachliche Wissensbausteine, Leitfäden, Grundlagen oder Begriffsklärungen.
- `templates/`: Vorlagen, Muster, Checklisten oder andere wiederverwendbare Arbeitsmittel.
- `evals/`: Testakten, Testprompts, Erwartungshorizonte, Scoring-Dateien und dokumentierte Ergebnisse.

Nicht jedes Modul muss von Anfang an alle diese Bestandteile enthalten. Manche Module beginnen mit einem Prompt, andere mit einer Wissensgrundlage, einer Vorlage oder einer Testakte.

## 3. Wofür steht `module_id`?

Die `module_id` verbindet Dateien, die zu einem konkreten fachlichen Modul gehören. Sie ist ein stabiler technischer Bezeichner innerhalb der Metadaten.

Beispiel:

```yaml
module_id: "markterkundung-it-beschaffung"
module: "markterkundung"
procurement_area: "it-beschaffung"
```

In diesem Beispiel bezeichnet `module_id` das konkrete Modul zur Markterkundung im Bereich IT-Beschaffung.

Das Feld `module` benennt den allgemeinen fachlichen Bereich. Das Feld `procurement_area` benennt den konkreten Beschaffungsbereich, auf den sich die Datei bezieht.

## 4. Allgemeine und spezifische Bausteine

Nicht alle fachlich verwandten Dateien müssen dieselbe `module_id` tragen. Allgemeine Wissensbausteine zur Markterkundung können zum Beispiel auch für andere Beschaffungsbereiche relevant sein.

Solche allgemeinen Bausteine können modulübergreifend nutzbar sein. Spezifische Bausteine, etwa eine Testakte zur IT-Beschaffung, können dagegen eine konkrete `module_id` verwenden, um ihre Zuordnung eindeutig zu machen.

## 5. Rolle der Evaluation

Evaluationsmaterialien dienen dazu, Prompts und KI-Assistenten unter vergleichbaren Bedingungen zu prüfen. Testakten enthalten dafür möglichst klar abgegrenztes Input-Material und konkrete Testprompts.

Erwartungshorizonte, Scoring-Dateien und Auswertungshinweise gehören nicht in den jeweils getesteten Assistenten. Sie dienen der späteren Bewertung. Dadurch können verschiedene Systeme blind und vergleichbar getestet werden.

## 6. Pflegehinweis

Kanonische Inhalte sollen im Repository möglichst an einer Stelle gepflegt werden. Das vermeidet widersprüchliche Versionen und reduziert Doppelpflege.

Die bestehende Struktur dient deshalb vor allem der Nachvollziehbarkeit, Pflege und Qualitätssicherung. Sie soll sichtbar machen, welche Dateien fachlich zusammengehören und welche Rolle sie im jeweiligen Modul erfüllen.
