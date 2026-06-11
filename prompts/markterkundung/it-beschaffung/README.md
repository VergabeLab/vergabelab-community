---
title: "README – Markterkundung IT-Beschaffung"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "module-readme"
license: "CC-BY-4.0"
repository_area: "prompts/markterkundung/it-beschaffung"
module_id: "markterkundung-it-beschaffung"
module: "markterkundung"
procurement_area: "it-beschaffung"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Community-Mitwirkende"
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Vergabepraktiker"
topics:
  - "Markterkundung"
  - "IT-Beschaffung"
  - "Readme"
  - "Hinweise"
  
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->
*VergabeLab Community – Wissensbaustein (Stand: Mai 2026) • © Okan Doğan • Lizenz: CC BY 4.0*

# Markterkundung IT-Beschaffung

Dieser Ordner enthält Hinweis- und Systemprompt-Bausteine für KI-Expertensysteme, die öffentliche Auftraggeber und Vergabestellen bei der **Vorbereitung, Durchführung und Auswertung von Markterkundungen** unterstützen.

Der Schwerpunkt liegt auf vergaberechtlichen Markterkundungen nach **§ 28 VgV** sowie – unterhalb der EU-Schwellenwerte – **§ 20 UVgO**. Die Bausteine sind besonders auf IT-Beschaffungen ausgerichtet, etwa Software, Hardware, Cloud-/SaaS-Leistungen, Schnittstellen, Datenschutz, IT-Sicherheit, Betrieb, Migration, SLAs und Lizenzmodelle.

Die Bausteine dienen der Strukturierung und Qualitätssicherung. Sie ersetzen keine Rechtsberatung im Einzelfall und automatisieren keine Vergabeentscheidung.

---

## Dateien in diesem Ordner

| Datei | Zweck | Einsatz |
|---|---|---|
| `01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md` | Hinweistext/Systemprompt für einen Markterkundungs-GPT | ChatGPT Custom GPT |

Weitere Varianten, etwa für Claude Projects oder andere KI-Systeme, können später ergänzt werden.

### Ergänzende Bausteine

Der Systemprompt ist für die gemeinsame Nutzung mit den folgenden VergabeLab-Bausteinen ausgelegt:

| Baustein                                                                                                                 | Funktion                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------- |
| [Leitfaden Markterkundung](../../../wissen/markterkundung/01_leitfaden_markterkundung_de.md)                             | Fachliche und methodische Grundlage für Planung, Durchführung, Auswertung und Dokumentation              |
| [Typische Fehler bei Markterkundungen](../../../wissen/markterkundung/02_typische_fehler_markterkundung_de.md)           | Prüf- und Risikobaustein, insbesondere zu Wettbewerb, Vorbefassung, Gleichbehandlung und Vertraulichkeit |
| [Anschreiben und Fragenkatalog](../../../templates/markterkundung/it-beschaffung/01_anschreiben_und_fragenkatalog_de.md) | Bearbeitbare Vorlage für die Kommunikation mit Marktteilnehmern                                          |

Bei der Einrichtung eines Custom GPT sollten diese Dateien zusätzlich als Wissensdateien hochgeladen werden.


---

## Schnellstart

Für die Einrichtung werden zwei Arten von Bausteinen verwendet:

* Der **Systemprompt** bestimmt Rolle, Arbeitsweise und Grenzen des Assistenten.
* Die **Wissens- und Template-Dateien** stellen die fachlichen VergabeLab-Inhalte bereit.

Für eine möglichst zuverlässige und konsistente Arbeitsweise sollten beide Bestandteile eingerichtet werden.

1. Öffne die Datei [`01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md`](./01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md).

2. Kopiere nur den Abschnitt zwischen **„KOPIERBEREICH START“** und **„KOPIERBEREICH ENDE“**.

3. Füge den kopierten Text in das Feld **„Hinweise“** beziehungsweise **„Instructions“** deines Custom GPT ein.

4. Lade zusätzlich folgende Dateien im ursprünglichen Markdown-Format (`.md`) herunter:

   * [`01_leitfaden_markterkundung_de.md`](../../../wissen/markterkundung/01_leitfaden_markterkundung_de.md)
   * [`02_typische_fehler_markterkundung_de.md`](../../../wissen/markterkundung/02_typische_fehler_markterkundung_de.md)
   * [`01_anschreiben_und_fragenkatalog_de.md`](../../../templates/markterkundung/it-beschaffung/01_anschreiben_und_fragenkatalog_de.md)

5. Lade diese drei Dateien im GPT-Editor unter **„Wissen“** beziehungsweise **„Knowledge“** hoch.

6. Ergänze bei Bedarf projektspezifische Rahmenbedingungen, etwa Bundesland, interne Vorgaben, Verwaltungsvorschriften oder besondere IT- und Sicherheitsanforderungen.

7. Teste den Assistenten anschließend in der Vorschau, zum Beispiel mit:

```text
Wir planen die Beschaffung einer Softwarelösung und möchten vorab eine Markterkundung durchführen. Bitte stelle mir die erforderlichen Rückfragen.
```

> **Hinweis:** Der Systemprompt kann auch allein verwendet werden. Ohne die ergänzenden Wissens- und Template-Dateien greift der Assistent jedoch stärker auf sein allgemeines Modellwissen zurück und kann die VergabeLab-Bausteine nicht gezielt berücksichtigen.

---

## Erwartete Arbeitsweise des Assistenten

Der Assistent arbeitet nach dem Prinzip:

> **Ask first, then draft.**

Das bedeutet: Bei unvollständigen Angaben soll der Assistent zunächst strukturierte Rückfragen stellen und nicht sofort vollständige Entwürfe erzeugen. Vollentwürfe, etwa Anschreiben, Fragenkataloge oder Auswertungsmatrizen, sollen erst erstellt werden, wenn der Sachverhalt hinreichend geklärt ist oder der Nutzer ausdrücklich einen Schnellstart wünscht.

Der Prompt enthält hierfür einen Gatekeeper mit zehn Pflichtangaben, unter anderem:

- Auftraggeber und Organisationseinheit,
- Leistungsbild,
- Schwellenwert-/Auftragswertkontext,
- Zeitplan,
- Stakeholder,
- Datenschutz- und Sicherheitsanforderungen,
- Schnittstellen,
- Betriebsmodell,
- Bestandssysteme und Migrationsbedarf,
- Budget- und Lizenzmodellannahmen.

---

## Typische Outputs

Der Markterkundungs-Assistent kann insbesondere folgende Arbeitsprodukte vorbereiten:

- strukturierte Rückfragen an den Auftraggeber,
- Zweck- und Dokumentationsvermerke zur Markterkundung,
- Musteranschreiben an Anbieter,
- Anbieter-Fragenkataloge,
- E-Mail-Entwürfe,
- Auswertungsmatrizen,
- Variantenvergleiche, etwa SaaS vs. On-Prem,
- Risikolisten für Leistungsbeschreibung, Auftragswert, Losbildung und Verfahrenswahl,
- Hinweise zur Neutralisierung von Vorbefassung.

---

## Vergaberechtliche Leitplanken

Bei der Nutzung ist insbesondere zu beachten:

- Markterkundungen dürfen nicht als Scheinausschreibungen oder verdeckte Preisabfragen ohne Beschaffungsabsicht genutzt werden.
- Gleichbehandlung, Transparenz und Wettbewerbsgrundsätze sind zu beachten.
- Anbieter sollten grundsätzlich identische Informationen erhalten, soweit dies für einen fairen Erkenntnisgewinn erforderlich ist.
- Vorbefasste Unternehmen sind nicht pauschal auszuschließen; ein möglicher Wissensvorsprung ist sachgerecht zu neutralisieren.
- Zweck, Auswahl der angesprochenen Unternehmen, Kommunikation, Unterlagen und Auswertung sollten dokumentiert werden.

Die Verantwortung für rechtliche Bewertung, Verfahrensgestaltung und Vergabeentscheidung bleibt immer beim Menschen.

---

## Datenschutz und Vertraulichkeit

Bitte keine personenbezogenen Daten, Betriebs- und Geschäftsgeheimnisse oder Details laufender Vergaben in öffentliche Systeme oder öffentliche Beiträge einfügen.

Für Tests und Community-Beiträge sollten Beispiele abstrahiert und anonymisiert werden, etwa mit Platzhaltern wie `[Auftraggeber]`, `[Projekt]`, `[Fachverfahren]`, `[Anbieter A]`.

---

## Hinweise für Beiträge

Verbesserungen sind willkommen, insbesondere:

- präzisere Rückfragen,
- bessere Struktur für IT-Markterkundungen,
- zusätzliche typische Schnittstellen oder Sicherheitsanforderungen,
- praxistaugliche Auswertungslogiken,
- Hinweise auf vergaberechtliche Risiken,
- bessere Formulierungen für Anschreiben oder Fragenkataloge.

Bitte beachte bei Beiträgen die allgemeinen Regeln in `CONTRIBUTING.md`, insbesondere:

- keine personenbezogenen Daten,
- keine vertraulichen Vergabeinformationen,
- keine fremden Texte ohne entsprechende Rechte,
- DCO-Sign-off für Pull Requests.

---

## Lizenz

Die Dateien in diesem Ordner stehen – soweit in der jeweiligen Datei nicht anders gekennzeichnet – unter **CC BY 4.0**.

Bitte beachte die jeweiligen SPDX- und Lizenzhinweise in den Dateien. Maßgeblich ist immer der konkrete Lizenzhinweis der jeweiligen Datei.
