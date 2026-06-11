---
title: "VergabeLab Community"
version: "0.2.0"
last_reviewed: "2026-06-07"
status: "initial"
language: "de-DE"
type: "root-readme"
license: "CC-BY-4.0"
repository_area: "root"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
topics:
  - "VergabeLab Community"
  - "KI-Bausteine"
  - "Vergabewesen"
  - "Wissen"
  - "Evaluation"
  - "Testakten"
  - "Netzwerk"
  - "Open Knowledge"
  - "Open Source"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

<img width="1200" height="410" alt="VergabeLab-Community" src="https://github.com/user-attachments/assets/1a2a22a4-b393-4b9e-9e3a-655342ba0a44" />

---
# VergabeLab Community - Freie KI-Bausteine für Vergabestellen

Dieses Repository sammelt **offene KI-Bausteine für das öffentliche Beschaffungswesen** – insbesondere Systemprompts und Konfigurationstexte, fachliche Wissensbausteine, Templates, Leitfäden sowie plattformneutrale Testakten und Evaluationsmaterialien. Die Bausteine können unter anderem in **ChatGPT Custom GPTs**, **Claude Projects und Skills** sowie anderen LLM-basierten Assistenzsystemen eingesetzt werden.

Inhaltlich reicht das Repository von der **Markterkundung** über **Leistungsbeschreibungen** bis hin zu **Vertragsgestaltung**, **Wertung**, **Dokumentation** und **Qualitätssicherung KI-gestützter Arbeitsabläufe**.

Ziel von VergabeLab Community ist es, **Erfahrungswissen aus der Praxis** in nachvollziehbare und wiederverwendbare Bausteine zu überführen und Vergabestellen bei der **sicheren und verantwortungsvollen Nutzung von KI** in Vergabeprozessen zu unterstützen.

**Was bringt das in der Vergabepraxis?**

* **Struktur und Tempo:** schneller vom „leeren Blatt“ zu belastbaren Entwürfen.
* **Qualitätssicherung:** weniger Lücken und Widersprüche, konsistentere Anforderungen und Kriterien.
* **Bessere Dokumentation:** nachvollziehbare Begründungs- und Dokumentationsbausteine.
* **Vergleichbare Tests:** fiktive Testakten und Bewertungsmaßstäbe für die strukturierte Prüfung unterschiedlicher KI-Systeme und Konfigurationen.

Der Fokus liegt ausdrücklich auf **Unterstützung**, nicht auf der Vollautomatisierung von Vergabeentscheidungen. Die Verantwortung für den konkreten Einsatz, die fachliche Prüfung und die daraus folgenden Entscheidungen bleibt beim Menschen.

> **Hinweis zur Nutzung:** Die Bausteine werden mit fachlicher Sorgfalt erstellt und vor ihrer Veröffentlichung geprüft. Diese Prüfung ist jedoch keine Zusicherung, dass ein Baustein für jeden Einzelfall vollständig, aktuell oder geeignet ist. Die Inhalte ersetzen weder die Prüfung des konkreten Beschaffungsvorgangs noch eine Rechtsberatung im Einzelfall. Bei KI-gestützter Nutzung können Ergebnisse zudem je nach Modell, Version, Konfiguration und Eingaben abweichen. Nutzung und Anpassung erfolgen daher in eigener Verantwortung. Es gelten die Gewährleistungs- und Haftungsregelungen der jeweils ausgewiesenen Lizenz; zwingende gesetzliche Haftung bleibt unberührt.

**Abgrenzung:** VergabeLab Community ist die Open-Knowledge- und Open-Source-Ebene dieses Projekts. Separate kommerzielle Angebote, etwa individuelle Anpassungen, Integrationsleistungen, Schulungen, Support oder Partner-Module, sind nicht Bestandteil dieses Repositorys und werden getrennt dokumentiert und vertraglich geregelt.

**Lizenzierung (Zusammenfassung):**  
- Alle **Textartefakte** in diesem Repository (Systemprompts/Hinweistexte, Templates, Guides, Muster, Wissensbausteine) stehen – soweit nicht in der Datei selbst anders gekennzeichnet – unter **CC BY 4.0** (Attribution, geringe Nutzungshürden).
- Echte **Software-/Tooling-Bestandteile** (z. B. Plugins, Skripte, Automatisierungstools) werden – sofern vorhanden – separat lizenziert und in einem eigenen Ordner (z. B. tooling/) geführt; hierfür ist **EUPL 1.2** vorgesehen.  
- Details, Pflichten und Beispiel-Attribution: siehe Abschnitt **[Lizenzierung](#5-lizenzierung)**.

---

## 1. Was finde ich hier konkret?

Beispiele für Bausteine, die hier nach und nach entstehen:

- **Markterkundung**  
  Systemprompts/Hinweistexte, mit denen KI-Assistenten strukturiert
  - Markterkundungen begleiten,
  - An Anbieter gerichtete Fragen formulieren,
  - Anbieter-Feedback zusammenfassen,
  - Risiken und Abhängigkeiten identifizieren.

- **Leistungsbeschreibungen**  
  Systemprompts/Hinweistexte, mit denen KI-Assistenten helfen,
  - technische und funktionale Anforderungen zu strukturieren,
  - Varianten- und Losbildung sauber abzubilden,
  - typische No-Gos (unzulässige Produkt-/Herstellervorgaben etc.) zu vermeiden.

- **Angebotswertung & Dokumentation**  
  Hilfen zur
  - Strukturierung von Zuschlagskriterien,
  - Dokumentation der Wertungsschritte,
  - Erzeugung von wertungsbegleitenden Begründungsbausteinen (ohne die Entscheidung zu „automatisieren“).

- **Muster-Dokumente (Wissensbasis)**  
  Leistungsfähige KI-Assistenten stehen und fallen mit der Wissensbasis. In diesem Repository sammeln wir daher auch
  - Muster-Anschreiben,
  - Muster-Fragenkataloge,
  - Muster-Leistungsbeschreibungen,
  - Vorlagen für Prüfschemata etc.

- **Begleitende Leitfäden**  
Kurze Handreichungen, wie die Bausteine
  - in Custom GPTs (chatgpt.com) und Pendants anderer Hersteller (z. B. Claude Projects),
  - in Azure OpenAI,
  - in selbst gehosteten LLM-Setups
eingebunden werden können.

* **Testakten und Evaluation**
  Unter [`evals/`](/evals/) entstehen plattformneutrale Testfälle, mit denen unterschiedliche KI-Assistenten, Prompts und Skills unter vergleichbaren Bedingungen geprüft werden können. Dazu gehören insbesondere

  * vollständig fiktive Input-Akten,
  * standardisierte Testprompts,
  * Erwartungshorizonte und Goldstandard-Outputschemata,
  * Scoring Rubrics und Auswertungshinweise,
  * Ergebnisordner für dokumentierte Testläufe.

  Der erste vollständige Evaluationsfall ist die [Testakte M-IT-01 zur Markterkundung bei einer IT-Beschaffung](/evals/markterkundung/it-beschaffung/M-IT-01/).


- **Software-Tools, Skripte und Automatisierung (perspektivisch)**  
  Künftig können auch echte Software- und Tooling-Bestandteile hinzukommen, etwa
  - kleine Hilfsskripte,
  - Prüf- oder Konvertierungswerkzeuge,
  - Integrationsbeispiele,
  - Automatisierungshilfen für wiederkehrende Arbeitsschritte.

  Solche Bestandteile werden getrennt von Textartefakten geführt (z. B. in `tooling/`) und gesondert lizenziert (EUPL 1.2).

---

## 2. Quickstart: So nutzt und testest du das erste Modul

> Für eine möglichst zuverlässige Arbeitsweise sollte nicht nur der Systemprompt eingerichtet werden. Zum Modul gehören auch fachliche Wissensbausteine, Templates und Testmaterialien.

**Beispiel: Markterkundung bei IT-Beschaffungen**

### I. Systemprompt auswählen

Öffne den Ordner [`prompts/markterkundung/it-beschaffung`](/prompts/markterkundung/it-beschaffung/) und anschließend die Datei [`01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md`](/prompts/markterkundung/it-beschaffung/01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md).

Kopiere nur den Abschnitt zwischen **„KOPIERBEREICH START“** und **„KOPIERBEREICH ENDE“**.

### II. KI-Assistent konfigurieren

Füge den kopierten Text in das Anweisungs- beziehungsweise Systemprompt-Feld des verwendeten KI-Systems ein.

Bei einem ChatGPT Custom GPT ist dies das Feld **„Hinweise“** beziehungsweise **„Instructions“**. Ergänze anschließend Name und Beschreibung des Assistenten.

### III. VergabeLab-Wissen und Template hinzufügen

Für die fachliche Unterfütterung sollten zusätzlich folgende Dateien im ursprünglichen Markdown-Format (`.md`) heruntergeladen und als Wissensdateien bereitgestellt werden:

* [`01_leitfaden_markterkundung_de.md`](/wissen/markterkundung/01_leitfaden_markterkundung_de.md)
* [`02_typische_fehler_markterkundung_de.md`](/wissen/markterkundung/02_typische_fehler_markterkundung_de.md)
* [`01_anschreiben_und_fragenkatalog_de.md`](/templates/markterkundung/it-beschaffung/01_anschreiben_und_fragenkatalog_de.md)

Der Systemprompt steuert Rolle und Arbeitsweise des Assistenten. Die Wissens- und Template-Dateien stellen die fachlichen VergabeLab-Inhalte und unmittelbar nutzbare Arbeitshilfen bereit.

### IV. Eigenen Kontext ergänzen

Ergänze bei Bedarf projektspezifische Rahmenbedingungen, etwa:

* Bundesland und anwendbare Verwaltungsvorschriften,
* Auftraggeber und Organisationseinheit,
* Beschaffungsgegenstand,
* interne IT- und Sicherheitsvorgaben,
* Datenschutzanforderungen,
* vorhandene Systeme und Schnittstellen.

Bitte keine personenbezogenen Daten, Betriebs- und Geschäftsgeheimnisse oder vertraulichen Informationen aus laufenden Vergabeverfahren in hierfür nicht freigegebene KI-Systeme eingeben.

### V. Assistent testen

Für einen einfachen Funktionstest kann beispielsweise folgende Eingabe verwendet werden:

```text
Wir planen die Beschaffung einer Softwarelösung und möchten vorab eine Markterkundung durchführen. Bitte stelle mir die erforderlichen Rückfragen.
```

Für einen strukturierten Vergleich steht zusätzlich die [Testakte M-IT-01](/evals/markterkundung/it-beschaffung/M-IT-01/) bereit.

Dabei gilt für Blindtests:

* Vorbereitung der Markterkundung: nur [Aktenstücke 01–05](/evals/markterkundung/it-beschaffung/M-IT-01/input/) verwenden;
* Auswertung der Marktrückläufe: [Aktenstücke 01–09](/evals/markterkundung/it-beschaffung/M-IT-01/input/) verwenden;
* [Aktenstücke 10–13](/evals/markterkundung/it-beschaffung/M-IT-01/expected/) nicht in den getesteten Assistenten laden, da sie Erwartungshorizont und Bewertungsmaßstab enthalten.

> **Community-Tipp:** VergabeLab-Bausteine sind bewusst so angelegt, dass sie angepasst, geprüft und verbessert werden können. Wenn du Änderungen oder Testergebnisse teilst, profitieren auch andere Nutzerinnen und Nutzer davon.

---

## 3. Struktur dieses Repositorys

Dieses Repository trennt fünf inhaltliche Ebenen:

1. Modellsteuerung,
2. fachliches Wissen,
3. wiederverwendbare Arbeitsmittel,
4. Nutzungs- und Integrationsanleitungen,
5. Evaluation und Qualitätssicherung.

Software- und Tooling-Bestandteile werden, sobald sie hinzukommen, getrennt von den Textartefakten geführt.

- **[`prompts/`](/prompts/)**  
  Systemprompts sowie Hinweis- und Konfigurationstexte zur Steuerung von LLM-basierten Assistenzsystemen. Die Dateien bestimmen insbesondere Rolle, Arbeitsweise, Grenzen und Ausgabeformate eines Assistenten.

- **[`wissen/`](/wissen/)**  
  Fachliche Wissensbasis und Referenzmaterialien, etwa Leitfäden, Grundlagen, Begriffsdefinitionen und typische Fehler. Diese Dateien können auch als Wissensdateien in KI-Systeme eingebunden werden.

- **[`templates/`](/templates/)**  
  Wiederverwendbare Muster und Arbeitsmittel für die Praxis, etwa Checklisten, Matrizen, Musteranschreiben, Fragenkataloge und Textbausteine.

- **[`guides/`](/guides/)**  
  Anleitungen zur Nutzung des Repositorys und zur Einbindung der Bausteine in unterschiedliche Systeme und Arbeitsabläufe.

  Weitere Hinweise dazu, wie einzelne Bausteine zu fachlichen Modulen zusammengefasst werden, finden sich im Guide [Modulstruktur in der VergabeLab Community](guides/02_modulstruktur_de.md).

- **[`evals/`](/evals/)**  
  Plattformneutrale Testfälle zur strukturierten Prüfung von Prompts, Custom GPTs, Skills und anderen KI-Assistenten. Testakten trennen regelmäßig zwischen Input-Material, Testprompts, internem Erwartungshorizont und dokumentierten Ergebnissen.

- **`tooling/` (perspektivisch)**  
  Künftiger Bereich für Software, Plugins, Skripte, Prüfwerkzeuge und andere ausführbare Artefakte. Solche Inhalte werden getrennt lizenziert.

- **[`LICENSES/`](/LICENSES/) und [`POLICIES/`](/POLICIES/)**  
  Lizenztexte, SPDX-Regeln und weitere projektweite Vorgaben. Maßgeblich sind die Lizenzhinweise in der jeweiligen Datei.

> Markdown-Dateien sollen grundsätzlich mit YAML-Frontmatter und einem SPDX-Kommentar versehen werden. Dadurch bleiben Lizenzzuordnung, Rechtekette, fachliche Einordnung und Verwendungszweck auch bei Kopie oder Weitergabe nachvollziehbar.

Die derzeitige Struktur stellt sich vereinfacht wie folgt dar:

```text
/
├─ prompts/
│  └─ markterkundung/
│     └─ it-beschaffung/
│        ├─ 01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md
│        └─ README.md
│
├─ wissen/
│  ├─ markterkundung/
│  │  ├─ 01_leitfaden_markterkundung_de.md
│  │  └─ 02_typische_fehler_markterkundung_de.md
│  └─ README.md
│
├─ templates/
│  └─ markterkundung/
│     └─ it-beschaffung/
│        └─ 01_anschreiben_und_fragenkatalog_de.md
│
├─ guides/
│  ├─ 00_github_basics_de.md
│  ├─ 01_lizenz_faq_de.md
│  └─ ...
│
├─ evals/
│  └─ markterkundung/
│     └─ it-beschaffung/
│        └─ M-IT-01/
│           ├─ README.md
│           ├─ input/
│           │  └─ Aktenstücke 01–09
│           ├─ prompts/
│           │  └─ Testprompts 01–05
│           ├─ expected/
│           │  └─ Aktenstücke 10–13
│           └─ results/
│
├─ LICENSES/
│  ├─ CC-BY-4.0.txt
│  └─ EUPL-1.2.txt
│
├─ POLICIES/
│  └─ SPDX.md
│
├─ CONTRIBUTING.md
├─ DCO.md
├─ index.html
└─ README.md
```
> **Experimentelle Leseschnittstelle**
> Unter api.vergabelab.de werden ausgewählte öffentliche Inhalte des Repositorys über eine statische Leseschnittstelle bereitgestellt. Die Schnittstelle befindet sich in einer experimentellen Phase. Sie ist derzeit keine (versionierte) Produkt-API; Inhalte, Pfade, Umfang und technische Struktur können sich jederzeit ändern. Es besteht kein Anspruch auf dauerhafte Verfügbarkeit oder Abwärtskompatibilität.

---

## 4. Wie kann ich beitragen?

Dieses Projekt lebt vom Erfahrungswissen der Community. Beiträge sind ausdrücklich erwünscht, egal ob du **Vergabepraktiker:in**, **Jurist:in** oder **Entwickler:in** bist. Du musst kein Git-Profi sein, um zu helfen!

### Neu bei GitHub?
- Wenn du GitHub nicht kennst, starte hier: [guides/00_github_basics_de.md](guides/00_github_basics_de.md).
- Alternativ reicht für den Anfang oft schon ein Beitrag in den **„Discussions“** (siehe unten).

### Wer ist angesprochen?
- **Öffentliche Auftraggeber & Vergabestellen** (Einbringen von Praxis-Perspektive, fachlichen Anforderungen etc.)
- **Rechtsberatung & Justiziariate** (Steigerung der Rechtssicherheit, Formulierungshilfen etc.)
- **Tech-Community** (Input bzgl. Integration, Prompt-Engineering, Automatisierung etc.)

### ⚠️ Bitte beachten (wichtig für Vergabestellen)
Damit **VergabeLab Community** öffentlich nutzbar bleibt, gilt:
* **Keine personenbezogenen Daten** (Namen, Kontaktdaten, Signaturen etc.).
* **Keine Details laufender Vergaben** und keine Betriebs- und Geschäftsgeheimnisse.
* Bitte nur **abstrahierte/anonymisierte Beispiele** („Bieter A/B“, „Projekt X“, „Leistungskategorie Y“).
* Falls interne Freigaben erforderlich sind: **bitte vor Veröffentlichung intern klären**.

### Wege der Mitarbeit

Es gibt drei Hauptwege, wie du dich einbringen kannst:

#### A. Der offene Weg: Discussions (Ideen, Fragen & Erfahrungsaustausch) 💬
Nutze die **"Discussions"** (den Reiter oben), für alles, was noch kein fester Arbeitsauftrag ist. Das ist unser Community-Forum.
- **Ideen einreichen:** Welche Anwendungsfälle fehlen noch (z. B. Bieterfragen & -antworten)?
- **Rechtliche Hinweise:** Gibt es neue Urteile oder Vorschriften, über die wir sprechen müssen?
- **Pilot-Feedback:** Teile deine Erfahrungen aus realen Projekten. Was spart Zeit? Wo entstehen Risiken?
> 👉 **[Direkt zu den Discussions](https://github.com/vergabelab/vergabelab-community/discussions)**

#### B. Der strukturierte Weg: Issues (Konkrete Fehler & Aufgaben) 🎯
Nutze die **"Issues"**, wenn du einen klaren Fehler gefunden hast oder ein konkretes Arbeitspaket vorschlagen möchtest.
- **Fehler melden:** Wo entstehen Missverständnisse oder Halluzinationen in einem bestimmten Prompt?
- **Konkrete Wünsche:** Anfragen für spezifische neue Templates, Leitfäden usw.
> 👉 **[Direkt zu den Issues](https://github.com/vergabelab/vergabelab-community/issues)**

#### C. Der direkte Weg: Pull Requests (Änderungen direkt umsetzen) 🛠️
Du fühlst dich sicher im Umgang mit GitHub? Dann freuen wir uns über direkte Verbesserungsvorschläge via **Pull Request**.
- **Hinweistexte/Systemprompts optimieren:** Bessere Formulierungen für bestehende Dateien.
- **Erweiterungen:** Neue fertige Bausteine für weitere Phasen des Vergabeprozesses hochladen.

**Hinweis:** Beiträge erfolgen standardmäßig per DCO (Signed-off-by). Pull Requests ohne Sign-off werden nicht gemergt (verpflichtender Check: **`DCO / DCO sign-off check`**). Details: [CONTRIBUTING.md](./CONTRIBUTING.md)


---

## 5. Lizenzierung
Dieses Repository enthält überwiegend Textartefakte, insbesondere Systemprompts und Hinweistexte, Templates, Guides, Muster, Wissensbausteine und Evaluationsmaterialien. Um die Nutzung in Vergabestellen und bei Partnern möglichst reibungsarm zu halten, sind Textartefakte grundsätzlich unter CC BY 4.0 lizenziert. Echte Software-/Tooling-Bestandteile (Code) werden – sofern vorhanden – separat behandelt.

### 5.1 Lizenz-Matrix (Ordner / typische Inhalte → Lizenz → Pflichten)

| Bereich/Ordner | Typische Inhalte | Lizenz | Kernpflichten |
|---|---|---|---|
| prompts/** | Systemprompts, Hinweistexte, Konfigurationstexte | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| wissen/** | Leitfäden, Grundlagen, Wissensbausteine, fachliche Referenzmaterialien | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| templates/** | Mustertexte, Vorlagen, Prüfschemata, Textbausteine | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| guides/** | Handreichungen, Anleitungen, Einbindungshinweise | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| evals/** | Fiktive Testakten, Testprompts, Erwartungshorizonte, Bewertungsraster und Auswertungshinweise | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| tooling/** (sofern vorhanden) | Code/Plugins/Skripte/Tools | EUPL 1.2 | Lizenz-/Copyright-Hinweise beibehalten; Bedingungen der EUPL 1.2 beachten |

**Vorrang von Datei-Hinweisen:** 
Soweit eine Datei einen YAML-Frontmatter + SPDX-Kommentar oder einen gleichwertigen Lizenzhinweis enthält, ist dieser für die jeweilige Datei maßgeblich.

### 5.2 Offizielle Lizenztexte

- **CC BY 4.0**: siehe `LICENSES/CC-BY-4.0.txt` sowie die offizielle Veröffentlichung:  
  https://creativecommons.org/licenses/by/4.0/
- **EUPL 1.2**: siehe `LICENSES/EUPL-1.2.txt` sowie die offizielle Veröffentlichung:  
  https://joinup.ec.europa.eu/collection/eupl/eupl-text-11-12
  
### 5.3 Praktische Hinweise:

**CC BY 4.0 (Textartefakte):**
- Bei Veröffentlichung/Weitergabe bitte Attribution (Projektname, Autor, Lizenz, Link) an geeigneter Stelle (z. B. Doku/Impressum/„Über“-Seite/Projektakte).
- Wenn du Inhalte bearbeitest, kennzeichne zusätzlich Änderungen knapp (z. B. „angepasst für Organisation/Abteilung X, Datum“).

**EUPL 1.2 (nur für `tooling/**`, sofern vorhanden):**
- Lizenz- und Urheberhinweise im Quelltext beibehalten.
- Bei Weitergabe, Bearbeitung oder öffentlicher Zugänglichmachung von EUPL-lizenzierten Softwarebestandteilen sind die Bedingungen der EUPL 1.2 zu beachten.

Weitere typische Fragen: siehe **[Lizenz-FAQ](./guides/01_lizenz_faq_de.md)**.

> Hinweis: Diese Hinweise sind eine pragmatische Orientierung. Maßgeblich sind die jeweiligen Lizenztexte sowie die Lizenzzuordnung je Datei.
---

## 6. Projektprinzipien & Fair-Use (nicht Teil der Lizenz)

Rechtlich maßgeblich sind ausschließlich die Lizenztexte und die Lizenzzuordnung je Datei (siehe Abschnitt **[Lizenzierung](#5-lizenzierung)**).  
Die folgenden Punkte sind **keine zusätzlichen Lizenzbedingungen**, sondern beschreiben, was VergabeLab unter einem fairen, community-orientierten Umgang versteht.

### Warum diese Lizenzierung?

Die VergabeLab Community soll in Vergabestellen und bei Partnern möglichst niedrigschwellig nutzbar sein. Deshalb stehen Textartefakte (inkl. Systemprompts/Hinweistexte) grundsätzlich unter **CC BY 4.0.** Daraus resultiert  eine klare Attributionspflicht, aber wenig Reibung innerhalb von Compliance-Prozessen.

Für echten Code/Tooling (sofern vorhanden) ist eine separate Lizenzierung vorgesehen (**EUPL 1.2**), um Softwarebestandteile sauber von Textartefakten zu trennen.

### Was wir als faire Nutzung verstehen

- **Transparenz statt "Black-Box"**  
  Wenn VergabeLab-Prompts/Hinweistexte in eigenen Systemen **verändert** und anschließend Dritten bereitgestellt werden, ist es im Sinne des Projekts, Verbesserungen wieder zugänglich zu machen (z. B. via Fork/Pull Request oder eigene Veröffentlichung unter kompatibler Lizenz).

- **Keine "stille" Übernahme als verdeckter Produktbestandteil**  
  VergabeLab soll nicht als unsichtbare Produktkomponente „mitlaufen“. Wer Inhalte produktiv – auch kommerziell – nutzt, sollte
  - die Herkunft transparent machen (Hinweis auf VergabeLab/Projekt-URL), und
  - Erkenntnisse/Verbesserungen möglichst zurückspielen.

- **Community first**  
  VergabeLab ist als Community-Projekt angelegt. Für Organisationen, die darüber hinaus Unterstützung benötigen (z. B. Anpassungen, Integrationskonzepte, Schulungen, Support), können Leistungen separat vertraglich vereinbart werden.

- **Respekt vor Urheberschaft und Lizenzhinweisen**  
  Bitte entferne bei eigenen Veröffentlichungen keine Hinweise auf Herkunft und Lizenz. Wo du darauf aufbaust, sollte erkennbar sein
  - dass die Basis aus der VergabeLab Community stammt, und
  - unter welcher Lizenz die abgeleiteten Inhalte stehen.
---

## 7. Empfohlener Urheberhinweis / Attribution
Soweit im Einzelfall nichts anderes vereinbart wird, freuen wir uns bei Nutzung von VergabeLab-Inhalten (z. B. in Custom GPTs, Fachverfahren oder Dokumentationen) über folgenden Hinweis:

```text
Basierend auf Bausteinen aus dem Open-Knowledge- und Open-Source-Projekt:
VergabeLab Community – KI-Bausteine für Vergabestellen
© 2026 Okan Doğan.
Lizenz: CC BY 4.0, sofern in der jeweiligen Datei nicht anders angegeben.
Für Code/Tooling im Ordner tooling/** gilt – sofern dort ausgewiesen – EUPL 1.2.
Projekt/Quelle: https://github.com/VergabeLab/vergabelab-community
Hinweis zu Änderungen: ggf. „Inhalte angepasst für [Organisation/Projekt], [Datum]“.
```
Der Hinweis kann z. B. in der technischen Dokumentation, im Impressum, in einer „Über dieses System“-Seite oder im Projektdokument platziert werden.

---
## 8. Über den Initiator
VergabeLab Community wurde von [Okan Doğan](https://github.com/raokandogan) ins Leben gerufen und mit ersten Prompts und Textbausteinen initial befüllt.

Als Fachanwalt für IT-Recht mit Schwerpunkt im Vergaberecht arbeitet Okan an der Schnittstelle von Digitalisierung, Legal Tech und öffentlicher Beschaffung. Sein Ziel ist es, öffentlichen Auftraggebern, Sektorenauftraggebern und Konzessionsgebern einen sicheren, rechtlich fundierten und pragmatischen Einstieg in die Nutzung von Künstlicher Intelligenz zu ermöglichen. 

Das Projekt ist aus der Überzeugung heraus entstanden, dass die Herausforderungen der KI-Adaption bei der öffentlichen Hand durch offenen Wissenstransfer und eine starke Community besonders gut angegangen werden können. Vernetz dich gerne oder tausche dich direkt aus: 
* **GitHub:** [@raokandogan](https://github.com/raokandogan)
* **LinkedIn:** [/ra-okan-dogan](https://de.linkedin.com/in/ra-okan-dogan)
* **Kanzlei:** [doganpfahler.de](https://doganpfahler.de/team/rechtsanwalt-okan-dogan/)

---
## Meldung von Rechts- und Urheberrechtsverletzungen (Notice and Takedown)

VergabeLab Community ist ein Open-Knowledge- und Open-Source-Projekt, das vom Erfahrungswissen und den Beiträgen seiner Nutzerinnen und Nutzer lebt. Wir nehmen den Schutz von Urheberrechten und geistigem Eigentum sehr ernst.

Alle Mitwirkenden bestätigen im Rahmen des DCO und der Projektregeln, dass sie nur Inhalte beisteuern, an denen sie die erforderlichen Rechte besitzen oder die sie rechtmäßig unter der jeweiligen Projektlizenz einreichen dürfen. Eine vollständige proaktive Prüfung sämtlicher Beiträge auf Rechte Dritter kann nicht erfolgen. Nachvollziehbaren Hinweisen auf mögliche Rechtsverletzungen gehen wir unverzüglich nach.

### So meldest du eine Rechtsverletzung

Solltest du der Ansicht sein, dass ein in diesem Repository veröffentlichter Textartefakt (Prompt, Musterdokument, Leitfaden etc.) deine Urheberrechte oder die Rechte deiner Organisation verletzt, bitten wir um einen kurzen, formlosen Hinweis. **Wir handeln unverzüglich.**

Bitte sende eine E-Mail an **kontakt [at] vergabelab [dot] de** mit folgenden Informationen:

* Einen direkten Link (URL) zu der betroffenen Datei oder dem Code-Abschnitt in diesem Repository.
* Eine kurze Erläuterung, warum der Inhalt deine Rechte verletzt (z. B. "Text wurde 1:1 aus unserem proprietären Leitfaden kopiert").
* Einen Nachweis deiner Urheberschaft oder Rechteinhaberschaft (z. B. Link zum Originaldokument).

**Ablauf:** Nachdem uns eine nachvollziehbare Beschwerde vorliegt, werden wir den betroffenen Inhalt im Sinne eines "Notice and Takedown"-Verfahrens unverzüglich entfernen oder unsichtbar schalten, bis der Sachverhalt abschließend geklärt ist. Von sofortigen anwaltlichen Abmahnungen bitten wir zur Schonung unnötiger Kosten und Ressourcen im Sinne der Open-Source-Community abzusehen.
