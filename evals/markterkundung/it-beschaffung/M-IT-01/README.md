---
title: "README – Fiktive Testakte M-IT-01 Markterkundung IT-Beschaffung"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "readme"
eval_case_id: "M-IT-01"
eval_role: "documentation"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/markterkundung/it-beschaffung/M-IT-01"

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

# README – Testakte M-IT-01

Diese Testakte dient dazu, KI-gestützte Bausteine für Markterkundungen bei öffentlichen IT-Beschaffungen realitätsnah zu testen. Sie kann insbesondere für ChatGPT Custom GPTs, Claude Skills, Agent-Skills und andere LLM-basierte Assistenten verwendet werden.

Die Testakte bildet bewusst **kein laufendes Vergabeverfahren** ab. Sie setzt in der vorgelagerten Phase an: Eine öffentliche Stelle hat einen fachlichen Bedarf, erste interne Vorstellungen und einzelne problematische Vorannahmen. Vor der Erstellung einer Leistungsbeschreibung soll geklärt werden, ob und wie der Markt neutral, transparent und dokumentationsfähig erkundet werden kann.

## Zeitliche Systematik

Die Testakte verwendet bewusst **keine realen Kalenderdaten**. Alle zeitlichen Angaben sind relativ zu `T0` zu lesen.

`T0` bezeichnet den Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam. Die Testakte soll nicht anhand des tatsächlichen Tagesdatums bewertet werden. Maßgeblich ist allein die interne relative Zeitachse der Akte.

| Zeitpunkt | Bedeutung |
|---|---|
| `T-6 Wochen` | Produktpräsentation eines bekannten Marktteilnehmers im Fachbereich |
| `T-3 Wochen` | informelles Angebot des Altanbieters, ein Grobkonzept zu erstellen |
| `T0` | Eingang der initialen Bedarfsmeldung einschließlich Bedarfserhebungsbogen |
| `T+1 Woche` | interne Sichtung durch Vergabestelle |
| `T+2 Wochen` | Abstimmung mit IT, Datenschutz und Kämmerei |
| `T+3 Wochen` | Entwurf der Markterkundung und Marktteilnehmerliste |
| `T+4 Wochen` | vorgesehener Versand der Markterkundung |
| `T+8 Wochen` | Eingang der Rückmeldungen |
| `T+10 Wochen` | Auswertung der Rückmeldungen |
| `T+12 Wochen` | Entscheidung über Beschaffungsstrategie und Mittelanmeldung |
| `T+20 Wochen` | frühestmöglicher Start eines Vergabeverfahrens |
| `T+36 Wochen` | frühestmöglicher Zuschlag |
| `T+12 Monate` | geplanter Produktivstart einer Pilotkommune |
| `T+18 Monate` | geplanter Rollout auf alle Trägerkommunen |

## Zweck des Tests

Der Testfall prüft, ob ein Assistent aus einer unvollständigen und teilweise risikobehafteten Ausgangslage eine vergaberechtlich strukturierte, neutrale und praktisch verwertbare Markterkundung entwickeln kann.

Der Assistent soll insbesondere erkennen und bearbeiten:

1. ob eine Markterkundung zweckmäßig ist und welche Anforderungen an Neutralität, Gleichbehandlung, Transparenz und Dokumentation bei ihrer Durchführung zu beachten sind;
2. welche Informationen vor Erstellung einer Leistungsbeschreibung fehlen;
3. welche internen Annahmen bereits zu produkt-, hersteller-, technologie- oder anbieterbezogen sind;
4. wie ein neutrales Markterkundungsanschreiben und ein verwertbarer Fragenkatalog formuliert werden können;
5. welche Risiken sich aus Datenschutz, IT-Sicherheit, Schnittstellen, Betriebsmodell, Migration, Lock-in, Barrierefreiheit und KI-Funktionen ergeben;
6. wie Rückmeldungen von Marktteilnehmern ausgewertet werden können, ohne eine verdeckte Wertung oder Vorentscheidung zu treffen;
7. welche Erkenntnisse später sachgerecht in Leistungsbeschreibung, Eignungsanforderungen, Zuschlagskriterien, Losbildung, EVB-IT-Vertrag und Vergabedokumentation einfließen können.

## Abgrenzung

Die Testakte ist ein Evaluationsfall für spezialisierte KI-Assistenten. Sie soll prüfen, ob ein Assistent eine Markterkundung in der vorgelagerten Beschaffungsphase sachgerecht vorbereitet, begleitet und auswertet.

Die Aufgabe des Assistenten besteht nicht darin, einen Anbieter auszuwählen, eine Zuschlagsentscheidung vorzubereiten oder eine bestimmte technische Lösung zu bevorzugen. Erwartet wird vielmehr, dass der Assistent die Markterkundung als **Vorbereitungsinstrument** behandelt: zur Klärung des Bedarfs, zur Strukturierung offener Fragen, zur Risikoerkennung, zur Neutralisierung möglicher Vorfestlegungen und zur nachvollziehbaren Dokumentation.

**Für Blindtests ist entscheidend:** Der Input richtet sich nach dem jeweiligen Testziel. Für Tests zur Vorbereitung der Markterkundung werden die **Aktenstücke 01–05** verwendet. Für Tests zur Auswertung der Marktrückläufe werden die **Aktenstücke 01–09** verwendet. Die **Aktenstücke 10–13** enthalten Erwartungshorizont, Musterlösung, Bewertungsraster und Hinweise zur Auswertung. Sie dienen ausschließlich der nachgelagerten Evaluation und dürfen nicht in den zu testenden Assistenten geladen werden.

## Empfohlene Test-Prompts

Die Testakte kann für unterschiedliche Testziele genutzt werden. Entscheidend ist, welche Aktenstücke dem zu testenden Assistenten als Input bereitgestellt werden.

Bei **Blindtests** bleiben die Aktenstücke 10–13 außerhalb des getesteten Systems. Bei Custom GPTs sollten sie insbesondere nicht als Knowledge-Dateien hochgeladen werden. Bei Claude Skills sollten sie nicht Bestandteil des Skill-Inputs oder der für den Skill bereitgestellten Testmaterialien sein.

### Test 1 – Aktenanalyse vor Durchführung der Markterkundung

**Input:** Aktenstücke 01–05

> Analysiere die Aktenstücke 01–05 aus Sicht einer Vergabestelle vor Einleitung eines Vergabeverfahrens. Prüfe, ob und wie eine Markterkundung durchgeführt werden sollte. Zeige vergaberechtliche Risiken, praktische blinde Flecken, problematische Vorfestlegungen und konkrete nächste Schritte.

### Test 2 – Neutrales Anschreiben und Fragenkatalog

**Input:** Aktenstücke 01–05

> Erstelle auf Basis der Aktenstücke 01–05 ein neutrales Markterkundungsanschreiben und einen strukturierten Fragenkatalog für Marktteilnehmer. Entferne unzulässige, suggestive oder vergaberechtlich riskante Formulierungen. Achte darauf, dass die Markterkundung der Vorbereitung der Beschaffung dient und keine Vorfestlegung auf bestimmte Anbieter, Produkte, Technologien oder Vertragsmodelle enthält.

### Test 3 – Auswertung der Marktrückläufe

**Input:** Aktenstücke 01–09

> Werte die Rückmeldungen der vier Marktteilnehmer aus. Erstelle eine neutrale Synopse und leite vergaberechtlich verwertbare Erkenntnisse für die spätere Beschaffung ab. Trenne klar zwischen belastbaren Markterkenntnissen, Einzelmeinungen einzelner Anbieter, offenen Klärungspunkten und riskanten Vorfestlegungen.

### Test 4 – Dokumentationsvermerk zur Markterkundung

**Input:** Aktenstücke 01–09

> Erstelle einen Vergabevermerk-Abschnitt zur Markterkundung. Dokumentiere Zweck, Ausgangslage, Vorgehen, angesprochene Marktteilnehmer, wesentliche Erkenntnisse, erkannte Risiken und empfohlene Folgeschritte. Achte darauf, dass der Vermerk keine Anbieterentscheidung vorwegnimmt und die spätere Leistungsbeschreibung neutral vorbereiten soll.

### Test 5 – Qualitätssicherung / Evaluation

**Input für den Assistenten:** je nach Testziel Aktenstücke 01–05 oder 01–09  
**Interne Auswertung:** Aktenstücke 10–13

> Prüfe die Antwort des Assistenten anhand des Erwartungshorizonts und des Bewertungsrasters. Bewertet werden insbesondere: vergaberechtliche Sensibilität, Neutralität der Markterkundung, Trennung von Bedarf und Lösung, Erkennung von Lock-in- und Datenschutzrisiken, Qualität des Fragenkatalogs, Dokumentationsfähigkeit und praktische Verwertbarkeit.

## Erwartete Kernleistung des Assistenten

Der Assistent soll nicht „den besten Anbieter“ auswählen und keine spätere Zuschlagsentscheidung vorbereiten. Die Markterkundung ist als **Vorbereitungsinstrument** zu behandeln.

Erwartet werden insbesondere:

- strukturierter Erkenntnisgewinn vor Einleitung des Vergabeverfahrens;
- neutrale und diskriminierungsfreie Ansprache des Marktes;
- Erkennung unzulässiger oder riskanter Vorfestlegungen;
- Trennung von Bedarf, Lösungsmöglichkeiten und Anbieterinteressen;
- Hinweise zu Datenschutz, IT-Sicherheit, Schnittstellen, Migration, Betrieb, Barrierefreiheit und Lock-in-Risiken;
- Ableitung neutraler Anforderungen für spätere Vergabeunterlagen;
- nachvollziehbare Dokumentation für die Vergabeakte.

## Nutzung mit Custom GPTs und Claude Skills

Die Testakte ist plattformneutral angelegt. Sie kann genutzt werden, um unterschiedliche KI-Setups mit demselben fachlichen Fall zu prüfen.

### Nutzung mit einem ChatGPT Custom GPT

Der Custom GPT sollte den eigentlichen Markterkundungs-Systemprompt bzw. Wissensbaustein enthalten. Die Testakte dient dagegen als **Testfall**.

Praktischer Ablauf:

1. Custom GPT mit dem Markterkundungs-Prompt konfigurieren.

2. Für einen Blindtest nur die passenden Input-Aktenstücke in den Chat mit dem GPT geben:

   * Vorbereitung der Markterkundung: Aktenstücke 01–05;
   * Auswertung der Marktrückläufe: Aktenstücke 01–09.

3. Einen der Testprompts aus dem Ordner [`prompts/`](./prompts/) verwenden.

4. Die Antwort getrennt vom getesteten Custom GPT auswerten.

   Für eine KI-gestützte Bewertung kann ein separater Evaluationschat oder ein eigener Evaluations-Assistent genutzt werden. Diesem Evaluationschat werden bereitgestellt:

   * der Output des getesteten Custom GPT;
   * die im Test verwendeten Input-Aktenstücke;
   * die Aktenstücke 10–13 als Erwartungshorizont und Bewertungsmaßstab.

   Wichtig: Die Aktenstücke 10–13 dürfen nicht vor oder während des Testlaufs in den zu testenden Custom GPT gelangen.

   Für wiederholbare Bewertungen sollte möglichst derselbe Evaluationsprompt verwendet werden, z. B.:

   > Bewerte den Output des getesteten Systems anhand der beigefügten Input-Aktenstücke sowie des Erwartungshorizonts und der Scoring Rubric aus den Aktenstücken 10–13. Erstelle keine eigene Musterlösung, sondern prüfe, inwieweit der Output die Bewertungskriterien erfüllt.


### Nutzung mit einem Claude Skill

Der Claude Skill sollte die Arbeitsweise für Markterkundungen enthalten, also Rolle, Prüfmethodik, Outputstruktur und Qualitätsanforderungen. Die Testakte dient als **Eval-Material** für diesen Skill.

Praktischer Ablauf:

1. Skill `markterkundung-it-beschaffung` bereitstellen.

2. Je nach Testziel nur die passenden Input-Aktenstücke als Testmaterial verwenden:

   - Vorbereitung der Markterkundung: Aktenstücke 01–05;
   - Auswertung der Marktrückläufe: Aktenstücke 01–09.

3. Den passenden Testprompt aus dem Ordner [`prompts/`](./prompts/) ausführen.

4. Die erzeugte Antwort getrennt vom getesteten Skill auswerten.

   Für eine KI-gestützte Bewertung kann ein separater Evaluationschat oder ein eigener Evaluations-Assistent genutzt werden. Diesem Evaluationschat werden bereitgestellt:

   - der Output des getesteten Skills;
   - die im Test verwendeten Input-Aktenstücke;
   - die Aktenstücke 10–13 als Erwartungshorizont und Bewertungsmaßstab.

   Wichtig: Die Aktenstücke 10–13 dürfen nicht vor oder während des Testlaufs in den zu testenden Skill gelangen.

   Für wiederholbare Bewertungen sollte möglichst derselbe Evaluationsprompt verwendet werden, z. B.:

   > Bewerte den Output des getesteten Systems anhand der beigefügten Input-Aktenstücke sowie des Erwartungshorizonts und der Scoring Rubric aus den Aktenstücken 10–13. Erstelle keine eigene Musterlösung, sondern prüfe, inwieweit der Output die Bewertungskriterien erfüllt.

## Hinweis zur Nutzung im Repository

Gewünschte Struktur und Ablageort für Testakten:

```text
evals/
  markterkundung/
    it-beschaffung/
      M-IT-01/
        README.md

        input/
          01_ausgangslage_bedarfsnotiz.md
          02_ist_landschaft_und_ziele.md
          03_bedarfsabfrage_fachbereich_ausgefuellt.md
          04_interner_entwurf_markterkundung_problematisch.md
          05_marktteilnehmerliste.md
          06_antwort_anbieter_a.md
          07_antwort_anbieter_b.md
          08_antwort_anbieter_c.md
          09_antwort_anbieter_d.md

        prompts/
          01_testprompt_vorbereitung_markterkundung_de.md
          02_testprompt_anschreiben_fragenkatalog_de.md
          03_testprompt_auswertung_marktruecklaeufe_de.md
          04_testprompt_dokumentationsvermerk_de.md
          05_testprompt_evaluation_de.md

        expected/
          10_erwartungshorizont_evaluation.md
          11_goldstandard_outputschema.md
          12_scoring_rubric.md
          13_hinweise_zur_auswertung.md

        results/
          .gitkeep
```

Die Testakte ist ein plattformneutraler Evaluationsfall. Der Bezug zu konkreten Implementierungen kann über Metadaten hergestellt werden, zum Beispiel:

```yaml
related_custom_gpt_prompt: "prompts/markterkundung/it-beschaffung/01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md"
target_systems:
  - "chatgpt-custom-gpt"
  - "claude-skill"
  - "generic-llm"
```
