---
title: "SPDX- und Metadaten-Policy"
version: "0.2.0"
last_reviewed: "2026-06-10"
status: "initial"
language: "de-DE"
type: "policy"
license: "CC-BY-4.0"
repository_area: "POLICIES"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
topics:
  - "SPDX"
  - "Lizenzierung"
  - "YAML-Frontmatter"
  - "Rechtekette"
  - "Quellenangaben"
  - "VergabeLab Community"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# SPDX- und Metadaten-Policy

## 1. Zweck

VergabeLab nutzt pro Datei einheitliche Metadaten und SPDX-Hinweise, damit Lizenz, Rechteinhaberschaft, Quellenstatus und Einordnung der Datei nachvollziehbar bleiben.

Der Standard lautet:

1. YAML-Frontmatter am Anfang der Datei,
2. danach ein SPDX-Kommentar,
3. anschließend der eigentliche Inhalt.

Dadurch bleibt die Datei sowohl für Menschen als auch für spätere Katalogisierung, Website-Sync, Suche oder Automatisierung gut auswertbar.

---

## 2. Grundstruktur je Markdown-Datei

Jede neue oder wesentlich geänderte Markdown-Datei soll am Anfang dieses Muster verwenden:

```md
---
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "..."
license: "CC-BY-4.0"
repository_area: "..."
spdx_file_copyright_text: "2026 Vorname Nachname"
spdx_license_identifier: "CC-BY-4.0"
---

<!--
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: CC-BY-4.0
-->
```

Für Software-/Tooling-Dateien gilt entsprechend die ausgewiesene Softwarelizenz, z. B.:
```md
---
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "tooling"
license: "EUPL-1.2"
repository_area: "tooling/..."
spdx_file_copyright_text: "2026 Vorname Nachname"
spdx_license_identifier: "EUPL-1.2"
---

<!--
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: EUPL-1.2
-->
```

### Modulgebundene Dateien

Modulgebundene Dateien sollen zusätzlich eine eindeutige Modulzuordnung erhalten:

```yaml
module_id: "markterkundung-it-beschaffung"
```

Die Felder `module_id`, `module` und `procurement_area` sind YAML-Frontmatter-Felder. Sie ersetzen den SPDX-Kommentar nicht.

Der Wert wird in `lowercase-kebab-case` geführt. Das Feld dient der eindeutigen Zuordnung fachlich zusammengehöriger Dateien und soll für modulgebundene Prompts, Wissensbausteine, Templates, Evaluationen und spätere Skill-Begleitdateien verwendet werden.

Für `SKILL.md` gilt der unten beschriebene Sonderstandard. Für allgemeine oder modulübergreifende Dateien ist `module_id` nicht erforderlich.

`module_id` ist nicht mit dem Dateipfad oder `repository_area` gleichzusetzen.

Beispiel:

```yaml
module_id: "markterkundung-it-beschaffung"
module: "markterkundung"
procurement_area: "it-beschaffung"
```

### Beschaffungsbereich

Der konkrete Beschaffungsbereich soll einheitlich mit `procurement_area` angegeben werden:

```yaml
procurement_area: "it-beschaffung"
```

Das bislang teilweise verwendete Feld `domain` soll künftig nicht synonym zu `procurement_area` verwendet werden.

In diesem Schritt werden noch keine bestehenden Fachdateien angepasst.

---

## 3. Verhältnis von YAML und SPDX-Kommentar

Die YAML-Felder dienen der strukturierten Metadatenpflege, Katalogisierung und späteren technischen Auswertung.

Der SPDX-Kommentar dient als klarer, dateibezogener Lizenz- und Rechtehinweis.

Wenn YAML-Metadaten und SPDX-Kommentar ausnahmsweise voneinander abweichen, ist die Abweichung vor dem Merge zu klären. Die Datei soll erst übernommen werden, wenn Lizenz und Rechteinhaberschaft eindeutig sind.

---

## 4. Pflichtangaben

Jede Markdown-Datei soll mindestens folgende YAML-Felder enthalten:

```yaml
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "..."
license: "..."
repository_area: "..."
spdx_file_copyright_text: "..."
spdx_license_identifier: "..."
```

Zusätzlich soll unmittelbar darunter ein SPDX-Kommentar stehen:

```md
<!--
SPDX-FileCopyrightText: <Jahr(e)> <Name des Rechteinhabers>
SPDX-License-Identifier: <Lizenz-ID>
-->
```

Zulässige Lizenz-IDs im Projekt sind insbesondere:

```md
CC-BY-4.0
EUPL-1.2
```

---

## 5. Typische Dateitypen

Für `type` sollen nach Möglichkeit einheitliche Werte verwendet werden:

```yaml
type: "root-readme"
type: "folder-readme"
type: "module-readme"
type: "guide"
type: "template"
type: "knowledge"
type: "systemprompt"
type: "policy"
type: "tooling"
type: "eval"
type: "eval-result"
```

Beispiele:

```yaml
type: "guide"
repository_area: "guides"
```

```yaml
type: "template"
repository_area: "templates/markterkundung/it-beschaffung"
```

```yaml
type: "knowledge"
repository_area: "wissen/markterkundung"
```

```yaml
type: "systemprompt"
repository_area: "prompts/markterkundung/it-beschaffung"
```

### Sonderfall `SKILL.md`

Eine portable Agent-Skill-Datei heißt `SKILL.md`. Sie verwendet ein mit der Agent-Skills-Spezifikation kompatibles YAML-Frontmatter.

Nach der allgemeinen Agent-Skills-Spezifikation sind mindestens folgende Top-Level-Felder erforderlich:

```yaml
name: "markterkundung-it-beschaffung"
description: "..."
```

VergabeLab legt ergänzend strengere projektinterne Pflichtangaben fest. Für jede VergabeLab-`SKILL.md` sind zusätzlich verpflichtend:

```yaml
license: "CC-BY-4.0"
metadata:
  author: "Okan Doğan"
  project: "VergabeLab Community"
  version: "0.1.0"
  vergabelab-status: "draft"
  vergabelab-language: "de-DE"
  vergabelab-module: "markterkundung"
  vergabelab-procurement-area: "it-beschaffung"
```

`author` bezeichnet die tatsächliche Person oder Organisation, die den Skill verfasst hat. Für den derzeitigen Stand ist dies `Okan Doğan`.

`project` bezeichnet die Zuordnung zum Projekt `VergabeLab Community`.

`version` bezeichnet die Version des konkreten Skills.

`vergabelab-status` beschreibt den Reife- beziehungsweise Bearbeitungsstand.

`vergabelab-language` bezeichnet die Inhaltssprache.

`vergabelab-module` bezeichnet den fachlichen Modulbereich.

`vergabelab-procurement-area` bezeichnet den konkreten Beschaffungsbereich.

Sämtliche Werte innerhalb von `metadata` werden als Strings geführt.

Der Wert von `name` muss dem Namen des übergeordneten Skill-Ordners entsprechen.

Zusätzliche VergabeLab-Felder wie `title`, `type`, `repository_area`, `skill_id` oder `skill_version` sollen nicht als eigene Top-Level-Felder in `SKILL.md` verwendet werden.

Das Feld `compatibility` bleibt optional und soll nur verwendet werden, wenn der Skill tatsächliche technische oder umgebungsbezogene Voraussetzungen besitzt, zum Beispiel:

```yaml
compatibility: "Erfordert Zugriff auf lokale Markdown-Referenzen."
```

Bei reinen Textskills ohne besondere technische Anforderungen soll `compatibility` entfallen.

Vollständiges Beispiel:

```yaml
---
name: "markterkundung-it-beschaffung"
description: "Unterstützt bei der Vorbereitung, Durchführung, Auswertung und Dokumentation von Markterkundungen bei öffentlichen IT-Beschaffungen."
license: "CC-BY-4.0"
metadata:
  author: "Okan Doğan"
  project: "VergabeLab Community"
  version: "0.1.0"
  vergabelab-status: "draft"
  vergabelab-language: "de-DE"
  vergabelab-module: "markterkundung"
  vergabelab-procurement-area: "it-beschaffung"
---
```

`SKILL.md` enthält im VergabeLab-Kontext textliche Skill-Anweisungen, Metadaten und Verweise. Diese Datei wird daher als Text-/Wissensartefakt behandelt.

Ausführbare Software- oder Tooling-Bestandteile innerhalb oder außerhalb eines Skill-Pakets sind gesondert zu kennzeichnen und nach der jeweils vorgesehenen Softwarelizenz zu führen.

Unmittelbar nach dem YAML-Frontmatter soll ein SPDX-Kommentar stehen:

```html
<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->
```

`author` und `SPDX-FileCopyrightText` erfüllen unterschiedliche Funktionen. `author` dient als beschreibende und in der GitHub-Vorschau sichtbare Metadatenangabe. Der SPDX-Kommentar dient als formalisierter dateibezogener Rechte- und Lizenzhinweis.

Beide Angaben müssen die tatsächliche Urheberschaft beziehungsweise Rechteinhaberschaft korrekt abbilden. Bei mehreren substantiell Beitragenden sind die bestehenden Regeln aus dieser Policy entsprechend anzuwenden.

Für andere Markdown-Dateien innerhalb eines späteren Skill-Bereichs gilt weiterhin der allgemeine VergabeLab-Metadatenstandard.

---

## 6. Wer steht im Copyright?

In den Rechtehinweis gehört die tatsächliche Person oder Organisation, die berechtigt ist, den Beitrag unter der angegebenen Lizenz bereitzustellen.

Die Angabe erfolgt an zwei Stellen:

1. im YAML-Frontmatter im Feld `spdx_file_copyright_text`,
2. im anschließenden SPDX-Kommentar als `SPDX-FileCopyrightText`.

Beide Angaben sollen inhaltlich übereinstimmen.

Beispiel:

```md
---
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "knowledge"
license: "CC-BY-4.0"
repository_area: "wissen/markterkundung"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->
```
Bei mehreren Rechteinhabern oder substantiellen Beiträgen mehrerer Personen sind mehrere SPDX-Zeilen zulässig:

```md
<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: CC-BY-4.0
-->
```
Im YAML-Frontmatter kann dies entsprechend als Textwert abgebildet werden:

```yaml
spdx_file_copyright_text: "2026 Okan Doğan; 2026 Vorname Nachname"
```

Alternativ kann bei künftiger technischer Auswertung eine Listenstruktur verwendet werden:

```yaml
spdx_file_copyright_text:
  - "2026 Okan Doğan"
  - "2026 Vorname Nachname"
```

Für den aktuellen Stand genügt ein einheitlicher Textwert. Wichtig ist, dass YAML und SPDX-Kommentar inhaltlich nicht widersprüchlich sind.

Bestehende Copyright-Zeilen dürfen nicht ohne Klärung entfernt werden.

---

## 7. Bearbeitungen

Bei bloßen redaktionellen Korrekturen muss nicht zwingend eine neue Copyright-Zeile ergänzt werden.

Bei substantiellen inhaltlichen Bearbeitungen kann eine zusätzliche Copyright-Zeile ergänzt werden. Bestehende Angaben bleiben erhalten.

Beispiel:

```md
<!--
SPDX-FileCopyrightText: 2025 Okan Doğan
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: CC-BY-4.0
-->
```

---

## 8. Keine exklusive Rechteübertragung

Durch das Einreichen eines Beitrags werden keine exklusiven Rechte an den Projektträger übertragen. Beiträge folgen dem Prinzip „Inbound = Outbound“: Ein Beitrag wird unter der Lizenz des betroffenen Ordners bzw. der betroffenen Datei veröffentlicht.

---

## 9. Zusicherung der Beitragenden

Mit jedem Beitrag bestätigen Beitragende, dass sie:

- die erforderlichen Rechte am eingereichten Inhalt besitzen oder zur Lizenzierung berechtigt sind,
- keine vertraulichen Informationen, personenbezogenen Daten oder Vergabeinterna einstellen,
- keine Betriebs- und Geschäftsgeheimnisse einstellen,
- keine urheberrechtlich geschützten Volltexte Dritter ohne ausreichende Berechtigung einstellen,
- fremde Inhalte, soweit sie verwendet werden, transparent kennzeichnen.

Pull Requests müssen per DCO signiert werden.

---

## 10. Quellenhinweise

Wenn Inhalte auf externen Quellen beruhen, sind diese Quellen transparent anzugeben.

Bei bloßer fachlicher Auswertung, Zusammenfassung oder Einordnung genügt regelmäßig ein sichtbarer Abschnitt am Ende der Datei:

```md
## Quellen

- [Titel der Quelle], [Autor/Herausgeber], [URL], abgerufen am [Datum]. Nutzung: fachliche Auswertung/Zusammenfassung/Zitat, keine Übernahme fremder Textpassagen.
```

Bei Übernahme, Bearbeitung oder Übersetzung fremder Inhalte müssen zusätzlich Rechte- und Lizenzstatus geprüft und angegeben werden.

Beispiel:

## Quellen- und Rechtehinweise

```md
- [Titel], [Autor/Herausgeber], [URL], abgerufen am [Datum]. Lizenz/Rechtestatus: [z. B. CC BY 4.0 / Nutzung mit Zustimmung / amtliches Werk / Zitat]. Änderungen: [gekürzt / zusammengefasst / übersetzt / sprachlich angepasst].
```
Fremde Inhalte dürfen nicht ohne passende Nutzungsrechte unter die VergabeLab-Lizenz gestellt werden.

---

## 11. Quellenangaben in YAML

Zusätzlich zum sichtbaren Quellenabschnitt können Quellen auch im YAML-Frontmatter erfasst werden:

```yaml
sources:
  - title: "Titel der Quelle"
    url: "https://..."
    author_or_publisher: "..."
    accessed: "2026-05-16"
    usage: "fachliche Auswertung/Zusammenfassung/Zitat, keine Textübernahme"
```

Die sichtbare Quellenangabe im Dokument bleibt bei Wissensbausteinen empfohlen, weil sie für Nutzerinnen und Nutzer unmittelbar nachvollziehbar ist.

---

## 12. Konfliktfall / Korrektur

Wenn Metadaten, SPDX-Kommentar, Lizenzangaben oder Quellenhinweise erkennbar fehlerhaft oder unklar sind, wird der Beitrag vor dem Merge korrigiert oder zurückgestellt, bis die Rechte- und Lizenzlage geklärt ist.

Typische Klärungsfälle:

- falscher Rechteinhaber,
- falsche Lizenz-ID,
- unklare Quelle,
- möglicher Fremdtext ohne Lizenzhinweis,
- personenbezogene Daten,
- Vergabeinterna,
- widersprüchliche YAML- und SPDX-Angaben.

---

## 13. Portabilität und kanonische Quellen

Inhalte sollen möglichst nicht manuell an mehreren Stellen parallel gepflegt werden.

Kanonische Quellen im Repository und daraus erzeugte portable Pakete können getrennt behandelt werden.

Konkrete Packaging-, Release- oder Build-Regeln sind noch nicht Gegenstand dieser Policy.
