---
title: "Testlauf M-IT-01 – Custom GPT API – Test 1 – Websuche aktiviert"
version: "0.1.0"
status: "completed"
language: "de-DE"
type: "eval-result"
subtype: "assistant-run"
eval_case_id: "M-IT-01"
eval_test_id: "test-1-vorbereitung-markterkundung"
run_id: "lauf-001"

tested_system: "ChatGPT Custom GPT"
tested_gpt: "Markterkundung by VergabeLab"
system_variant: "API Actions"
web_search_enabled: true
actions_enabled: true
knowledge_files_uploaded: false

test_mode: "exploratory-practice-test"
blind_test_status: "limited"
blind_test_note: "Die Expected-Dateien 10–13 wurden nicht als Input bereitgestellt. Da die Websuche aktiviert war und das Repository öffentlich ist, kann ein Zugriff über die Websuche methodisch nicht vollständig ausgeschlossen werden."

run_date: "2026-06-07"
relative_date: "T+10 Wochen"
evaluator: "Okan Doğan"

prompt_version: "0.1.1"
repository_commit: "f74bb02"
action_base_url: "https://api.vergabelab.de"

score_total: 96
score_maximum: 100
score_classification: "sehr gut"

data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/markterkundung/it-beschaffung/M-IT-01/results"

spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
---

<!-- SPDX-FileCopyrightText: 2026 Okan Doğan -->

<!-- SPDX-License-Identifier: CC-BY-4.0 -->

# Testlauf M-IT-01 – Custom GPT API – Test 1

## 1. Zweck des Testlaufs

Dieser Testlauf prüft, ob der VergabeLab Custom GPT die Aktenstücke 01–05 aus Sicht einer Vergabestelle zutreffend analysiert und daraus eine neutrale, dokumentationsfähige und vergaberechtlich belastbare Markterkundungsstrategie ableitet.

Geprüft werden insbesondere:

* vergaberechtliches Grundverständnis;
* Erkennung offener Informationsbedarfe;
* Identifikation von Vorfestlegungen und Risiken;
* Trennung von Bedarf, Markterkundung und späterem Vergabeverfahren;
* praktische nächste Schritte;
* Nutzbarkeit der Antwort für Vergabestelle und Projektgruppe.

## 2. Testkonfiguration

| Merkmal                        | Konfiguration                |
| ------------------------------ | ---------------------------- |
| System                         | ChatGPT Custom GPT           |
| GPT                            | Markterkundung by VergabeLab |
| Wissensbereitstellung          | VergabeLab Actions           |
| Action-Endpunkt                | `https://api.vergabelab.de`  |
| Websuche                       | aktiviert                    |
| Hochgeladene Knowledge-Dateien | keine                        |
| Eingabedateien                 | Aktenstücke 01–05            |
| Nicht als Input verwendet      | Aktenstücke 06–13            |
| Systemprompt-Version           | `0.1.1`                      |
| Repository-Commit              | `f74bb02`                    |
| Testdatum                      | 07.06.2026                   |

### Verwendete Input-Aktenstücke

1. `01_ausgangslage_bedarfsnotiz.md`
2. `02_ist_landschaft_und_ziele.md`
3. `03_bedarfsabfrage_fachbereich_ausgefuellt.md`
4. `04_interner_entwurf_markterkundung_problematisch.md`
5. `05_marktteilnehmerliste.md`

### Expected-Dateien

Die Aktenstücke 10–13 wurden nicht als Eingabedateien bereitgestellt.

Da die Websuche aktiviert war und das Repository öffentlich ist, wird dieser Lauf nicht als vollständig abgeschotteter Blindtest, sondern als explorativer Praxistest dokumentiert. Ein zusätzlicher Referenzlauf mit deaktivierter Websuche ist vorgesehen.

## 3. Verwendeter Testprompt

```text
Analysiere die Aktenstücke 01–05 aus Sicht einer Vergabestelle vor Einleitung eines Vergabeverfahrens. Prüfe, ob und wie eine Markterkundung durchgeführt werden sollte. Zeige vergaberechtliche Risiken, praktische blinde Flecken, problematische Vorfestlegungen und konkrete nächste Schritte.
```

## 4. Beobachtete Quellen- und Werkzeugnutzung

Soweit in der Aktivitätsanzeige nachvollziehbar:

* VergabeLab-Action `getMarkterkundungLeitfaden`: aufgerufen
* VergabeLab-Action `getMarkterkundungFehlercheck`: aufgerufen
* VergabeLab-Action `getMarkterkundungTemplate`: nicht aufgerufen
* Websuche: aktiviert
* Externe Webquellen in der Antwort: keine

## 5. Unveränderte Antwort des Assistenten

> Die nachfolgende Antwort wird unverändert dokumentiert. Rechtschreibung, Struktur und Formulierungen werden nicht nachträglich korrigiert.

```markdown
# Gesamtbewertung

**Eine strukturierte Markterkundung sollte durchgeführt werden.** Sie ist hier nicht nur zweckmäßig, sondern praktisch erforderlich, um den Beschaffungsgegenstand neutral und ausschreibungsreif zu bestimmen, den Auftragswert zu plausibilisieren, die Losbildung zu untersuchen und die geeignete Verfahrensart festzulegen.

Die Akte enthält bereits eine gute Ausgangsbasis: fachliche Ziele, Fallzahlen, Ist-Systeme, Schutzbedarfe und unterschiedliche Lösungsansätze sind erkennbar. Es fehlen aber belastbare Informationen zu Schnittstellen, Migration, Betriebsmodellen, Marktbreite, Kostenparametern und Eigenaufwand. Zugleich bestehen erhebliche Risiken eines Produkt- und Herstellerzuschnitts durch die frühere Produktpräsentation und das Konzeptangebot des Bestandsanbieters.  

Der Entwurf in Aktenstück 04 sollte **nicht versendet** werden. Er vermischt Markterkundung, unverbindliche Angebotsabfrage, Konzeptwettbewerb und eine mögliche spätere Anbieterbewertung. Damit drohen ein verzerrtes Marktbild, ungleiche Vorbefassung und eine spätere angreifbare Leistungsbeschreibung. 

Rechtlicher Rahmen sind insbesondere § 28 VgV, § 7 VgV, § 3 VgV, § 8 VgV sowie die Grundsätze aus § 97 GWB. Die Markterkundung muss dem Vergabeverfahren vorgelagert bleiben. Sie darf weder eine Scheinausschreibung noch eine verdeckte Angebots- oder Konzeptwertung sein.

## 1. Bewertung der einzelnen Aktenstücke

### Aktenstück 01 – Ausgangslage und Bedarfsnotiz

**Positiv**

Die Zwecke der Markterkundung sind im Kern richtig bestimmt:

* Ermittlung marktgängiger Lösungsansätze,
* Vorbereitung einer funktionalen Leistungsbeschreibung,
* Klärung von Schnittstellen, Migration und Betrieb,
* Plausibilisierung von Kosten und Lizenzmodellen,
* Vorbereitung der Losbildungsentscheidung.

Der Zeitplan trennt Markterkundung und Vergabeverfahren ausreichend deutlich. Auch der Budgetkorridor wird zutreffend als vorläufig und nicht als Marktpreis behandelt. 

**Risiken und offene Punkte**

Die Beschaffungseinheit ist noch nicht eindeutig definiert. Offen bleibt, ob beschafft werden soll:

* ein Fachportal,
* eine Plattform einschließlich Prozessimplementierung,
* ein Portal mit Integrations- und Migrationsleistungen,
* oder ein über mehrere Jahre fortzuentwickelnder Managed Service.

Diese Varianten sind kosten-, wettbewerbs- und risikoseitig kaum vergleichbar. Ohne Referenzumfang würden Anbieter bei einer Preisabfrage unterschiedliche Leistungsbilder kalkulieren.

Die interkommunale Struktur ist ebenfalls beschaffungsrelevant. Vor der Marktansprache sollte geklärt werden:

* welche Rechtsträger Vertragspartner werden,
* welche Kommunen verbindlich teilnehmen,
* welche Abruf- oder Erweiterungsoptionen vorgesehen sind,
* welche Mengen und Nutzerzahlen gesichert beziehungsweise optional sind,
* wer Verantwortlicher im datenschutzrechtlichen Sinne ist.

**Bewertung:** tragfähige Ausgangsnotiz, aber noch kein ausreichend bestimmter Informationsstand für eine externe Marktansprache.

---

### Aktenstück 02 – IT-Ist-Landschaft, Ziele und offene Punkte

Dieses Aktenstück ist die stärkste fachlich-technische Grundlage der Akte. Besonders hilfreich sind die Nicht-Ziele, die verschiedenen Lösungsansätze und die bereits benannten Lock-in-, Datenschutz- und Schnittstellenrisiken. 

**Wesentliche blinde Flecken**

1. **Schnittstellen sind nur nominell beschrieben.**
   „REST-API vorhanden“, „SOAP eingeschränkt“ und „CSV-Import möglich“ reichen für belastbare Marktaussagen nicht. Benötigt werden mindestens Datenobjekte, zulässige Schreibrichtungen, Authentisierung, Mengengerüste, Frequenzen, Herstellerfreigaben und bekannte Lizenzbeschränkungen.

2. **Die Rolle des Fachverfahrens bleibt unklar.**
   Es ist nicht entschieden, ob das Portal nur Daten übergibt, das führende Vorgangssystem wird oder einen eigenen Workflow einschließlich Bescheidvorbereitung betreibt. Diese Architekturentscheidung beeinflusst Produktangebot, Migration, Datenschutz, Preis und Losbildung fundamental.

3. **Identitäts- und Zugangskonzept fehlt.**
   Für Sorgeberechtigte, Schulen, Dienstleister und interne Beschäftigte bestehen unterschiedliche Authentisierungs- und Berechtigungsanforderungen. Die bloße Nennung von SAML/OIDC und einer geplanten BundID-Anbindung reicht nicht.

4. **Nichtfunktionale Anforderungen fehlen weitgehend.**
   Noch zu bestimmen beziehungsweise am Markt zu plausibilisieren sind insbesondere:

   * Verfügbarkeit und Servicezeiten,
   * Reaktions- und Wiederherstellungszeiten,
   * RTO/RPO,
   * erwartete Spitzenlasten,
   * Protokollierung und Monitoring,
   * Mandantentrennung,
   * Backup und Wiederanlauf,
   * Schwachstellen- und Patchmanagement,
   * Anforderungen an Penetrationstests,
   * Exit- und Übergangsleistungen.

5. **Barrierefreiheit ist zu abstrakt.**
   Zu klären sind der anzuwendende Rechts- und Prüfmaßstab, Nachweise, Testverfahren und die Behandlung barrierefreier Dokumente und Formulare.

6. **Die E-Akte ist noch nicht architektonisch entschieden.**
   Dadurch ist offen, ob Anbieter verbindlich DMS-Integration, revisionssichere Ablage oder nur Exporte kalkulieren sollen.

**Bewertung:** sehr gute Themenliste, aber vor Versand muss daraus eine neutrale System- und Prozessbeschreibung mit klaren Annahmen werden.

---

### Aktenstück 03 – Bedarfserhebungsbogen

Der Bedarfserhebungsbogen dokumentiert den fachlichen Schmerzpunkt plausibel und unterscheidet grundsätzlich zwischen Muss-, Soll- und Wunschmerkmalen. Positiv ist auch, dass die Datenlage und die fehlende technische Prüfung offen benannt werden. 

**Problematische Vorfestlegungen**

* „möglichst aus einer Hand“,
* bereits vorkonfigurierte schulbezogene Prozesse,
* Einsatz bei anderen Kommunen im Schulbereich,
* SaaS aus EU-Rechenzentren,
* möglichst wenig eigene IT-Betriebsverantwortung,
* sehr kurze Einführungszeit.

Jede dieser Präferenzen kann sachlich begründbar sein. Der Akte fehlt bislang aber die Prüfung, ob sie tatsächlich funktional erforderlich ist oder lediglich auf organisatorischer Bequemlichkeit beziehungsweise dem Eindruck der Produktdemo beruht.

Besonders kritisch ist die Vermischung von **Bedarf** und **Lösungsweg**:

* Der Bedarf lautet beispielsweise geringe interne Betriebsbelastung.
* Daraus folgt nicht automatisch SaaS.
* Der Bedarf lautet geringe Konfigurations- und Entwicklungsbelastung.
* Daraus folgt nicht automatisch ein fertiges Fachportal.
* Der Bedarf lautet klare Gesamtverantwortung.
* Daraus folgt nicht automatisch eine vergaberechtlich zulässige Gesamtvergabe.

**Weitere blinde Flecken**

Die Fallzahlen sind nur Schätzungen. Für die Markterkundung sollten zumindest plausibilisiert werden:

* Fallzahlen pro Leistung und Mandant,
* saisonale Spitzen,
* Dokumentenvolumen und Dateigrößen,
* Zahl paralleler interner und externer Nutzer,
* Kommunikationsvorgänge,
* Anzahl von Formularen, Prozessvarianten und Bescheidtypen,
* erwartete Wachstums- und Erweiterungsoptionen.

Ohne diese Mengengerüste sind Preisindikationen wenig vergleichbar.

**KI-Funktionen**

Die KI-Wünsche sollten nicht als einheitlicher Funktionsblock abgefragt werden. Zu unterscheiden sind:

* Dokumentenklassifikation,
* Datenextraktion,
* Textvorschläge,
* Chatbot oder Auskunftssystem,
* Entscheidungsunterstützung,
* automatisierte Entscheidung.

Für jede Funktion wären Datenflüsse, menschliche Kontrolle, Trainings- und Nutzungszwecke, Protokollierung, Modellanbieter, Datenresidenz sowie Rollen nach der KI-Verordnung gesondert zu betrachten. Zum derzeitigen Stand sollten KI-Funktionen eher als **optionaler Marktbeobachtungsblock** und nicht als prägender Kern des Beschaffungsgegenstands behandelt werden.

---

### Aktenstück 04 – Problematischer Markterkundungsentwurf

Der Entwurf ist in seiner aktuellen Fassung vergaberechtlich und methodisch nicht verwendbar. 

#### „Gesamtlösung aus einer Hand“

Diese Formulierung legt eine Gesamtvergabe nahe, bevor die fachliche und technische Losbildung überhaupt untersucht wurde. Sie bevorzugt größere Generalanbieter und kann spezialisierte Portal-, Integrations-, Migrations- oder Betriebsanbieter von einer Beteiligung an der Markterkundung abhalten.

**Korrektur:** funktional fragen, welche Verantwortungs- und Leistungsschnitte marktgängig sind, welche Abhängigkeiten bestehen und unter welchen Voraussetzungen eine Losbildung oder Gesamtvergabe praktikabel wäre.

#### Bezug auf eine bereits gesehene Produktpräsentation

Der Hinweis, eine konkrete Präsentation bilde viele Anforderungen gut ab, signalisiert den Marktteilnehmern einen bereits vorhandenen Referenzmaßstab. Zugleich bestätigt er die Beeinflussung des Fachbereichs.

**Korrektur:** vollständig streichen. Die frühere Präsentation ist intern als mögliche Vorbefassung und Erkenntnisquelle zu dokumentieren, nicht als Orientierung für andere Unternehmen zu kommunizieren.

#### „Vergleichbare Lösungen“

Die Aufforderung, vergleichbare Lösungen anzubieten, kann dazu führen, dass alle Antworten auf das bereits bekannte Produktmodell ausgerichtet werden. Alternative Architekturansätze werden dadurch entwertet.

**Korrektur:** die zu lösenden fachlichen, technischen und betrieblichen Probleme beschreiben und ausdrücklich mehrere Lösungsansätze zulassen.

#### Konzeptskizze, Architektur und Einführungsplan

Eine kurze Darstellung des Lösungsansatzes ist zulässig und sinnvoll. Die hier verlangte Tiefe nähert sich aber einer unentgeltlichen Beratungs- oder Angebotsleistung.

**Korrektur:** strukturierte Angaben auf einer vorgegebenen Abstraktionsebene verlangen. Keine individuell ausgearbeitete Zielarchitektur und kein Feinkonzept.

#### „Belastbare“ oder „möglichst verbindliche“ Preise

Eine Markterkundung darf unverbindliche Preisindikationen, Korridore und Preisbildungsparameter erheben. Verbindliche Kostenschätzungen für ein noch unbestimmtes Leistungsbild sind weder methodisch sinnvoll noch sauber von einem Angebot abgrenzbar.

**Korrektur:** Kostenkorridore mit Annahmen, Preistreibern, einmaligen und laufenden Kosten sowie möglichen Mengeneinheiten abfragen.

#### Offenlegung des Budgetrahmens

Die Nennung von 850.000 bis 1.400.000 Euro kann Antworten am verfügbaren Budget verankern. Unternehmen könnten Leistungsumfang und Preis auf diesen Korridor zuschneiden.

**Korrektur:** zunächst ohne Budgetvorgabe erheben. Falls der Markt ohne Budgetinformation keine sinnvollen Varianten benennen kann, kann in einer zweiten Stufe eine Größenklasse oder Finanzierungsgrenze transparent und gleichlautend kommuniziert werden. Die Entscheidung ist zu dokumentieren.

#### „Besonders überzeugende Konzepte“

Diese Formulierung ist besonders kritisch. Sie erweckt den Eindruck, Beiträge der Markterkundung würden für die spätere Beschaffung bewertet oder verschafften Vorteile.

**Korrektur:** ausdrücklich klarstellen, dass Teilnahme, Nichtteilnahme sowie Inhalt und Umfang der Antwort weder die Teilnahmechancen noch die spätere Wertung beeinflussen.

#### 70-Prozent-Standardabdeckung

Die Bezugsgröße ist nicht definiert. Zudem fördert die Prozentfrage Marketingangaben statt vergleichbarer Erkenntnisse.

**Korrektur:** Anforderungen oder Prozessbausteine einzeln als Standard, Konfiguration, Erweiterung, Individualentwicklung oder nicht verfügbar einordnen lassen.

#### Kompatibilität mit `DMS-Nord` und `SchulFach 9`

„Kompatibel“ ist zu unbestimmt und lädt zu unbelegten Ja-Antworten ein.

**Korrektur:** konkret abfragen:

* vorhandener Standardkonnektor,
* dokumentierte Referenzintegration,
* Nutzung offener Schnittstellen,
* erforderliche Drittanbieterleistungen,
* geschätzter Anpassungsaufwand,
* technische und lizenzrechtliche Voraussetzungen.

#### Ausschluss von Drittstaatenverarbeitung

Das kann ein legitimes Schutzbedürfnis sein, ist aber gegenwärtig weder datenschutzrechtlich noch technisch ausreichend operationalisiert. Unklar ist, ob nur Primärdaten, auch Metadaten, Telemetrie, Supportzugriffe, Unterauftragnehmer und Administrationszugriffe gemeint sind.

**Korrektur:** Datenflüsse, Verarbeitungsorte, Unterauftragnehmer, Fernzugriffe, Support und eingesetzte Cloud- beziehungsweise KI-Dienste strukturiert offenlegen lassen. Die endgültige Mindestanforderung ist anschließend mit Datenschutz und IT-Sicherheit festzulegen.

#### Kostenfreies Feinkonzept

Diese Frage sollte gestrichen werden. Sie fordert eine erhebliche Vorleistung, begünstigt Anbieter mit hohen Presales-Kapazitäten und erhöht das Vorbefassungs- und Verwertungsrisiko.

#### Produktpräsentationen

Produktdemos können Erkenntnisse liefern, dürfen aber keine unstrukturierten Vertriebsgespräche sein.

**Korrektur:** erst nach Auswertung schriftlicher Antworten, gleiche Agenda und Zeit, identische Use Cases, dokumentierte Fragen und keine „Schönheitsbewertung“ der Produktoberfläche.

---

### Aktenstück 05 – Marktteilnehmerliste

Die Liste bildet unterschiedliche Marktsegmente ab und behandelt den Bestandsanbieter nicht automatisch als ausgeschlossen. Das ist grundsätzlich richtig. Auch die vorgesehenen gleichen Unterlagen und die neutrale Synopse sind sachgerecht. 

**Die Marktbreite ist dennoch nicht ausreichend belastbar.**

Vier gezielt ausgewählte Unternehmen können bei einem voraussichtlich EU-weiten IT-Vorhaben ein zu enges Marktbild liefern. Es besteht insbesondere die Gefahr, dass die Marktsegmente zwar abstrakt unterschiedlich erscheinen, die tatsächliche europäische Anbieterlandschaft aber nicht abgedeckt wird.

Empfehlenswert ist eine Kombination aus:

* dokumentierter eigener Markt- und Referenzrecherche,
* Erfahrungsaustausch mit anderen öffentlichen Auftraggebern,
* offener Bekanntmachung oder Interessenbekundungsmöglichkeit,
* ergänzender direkter Ansprache sachgerecht ausgewählter Unternehmen.

Die offene Veröffentlichung ist nicht zwingend, reduziert hier aber das Risiko einer selektiven Auswahl und ermöglicht bislang unbekannten Anbietern, Integratoren oder Konsortien die Beteiligung.

**Anbieter D / Bestandsanbieter**

Anbieter D darf nicht allein aufgrund seiner Bestandsrolle ausgeschlossen werden. Das angebotene kostenlose Grobkonzept sollte jedoch in dieser Form nicht angenommen werden.

Zunächst ist aktenkundig festzuhalten:

* welche Gespräche bereits stattgefunden haben,
* welche Informationen Anbieter D erhalten hat,
* welche Informationen oder Lösungsideen von ihm stammen,
* welche technischen Kenntnisse nur der Bestandsanbieter besitzt,
* ob bestehende Vertrags-, Lizenz- oder Schnittstellenrechte Wettbewerber faktisch benachteiligen.

Erforderliche Informationen sind anschließend zu neutralisieren und allen späteren Teilnehmern zugänglich zu machen. Ein Ausschluss wäre nur letztes Mittel, wenn ein Wettbewerbsvorteil nicht durch Wissensausgleich, neutrale Unterlagen und angemessene Fristen beseitigt werden kann.

## 2. Zentrale Risikobewertung

| Risiko                                      |       Bewertung | Erforderliche Maßnahme                                                               |
| ------------------------------------------- | --------------: | ------------------------------------------------------------------------------------ |
| Produktzuschnitt nach früherer Demo         |            hoch | Demo, Inhalte und interne Folgerungen dokumentieren; Anforderungen funktionalisieren |
| Vorbefassung des Bestandsanbieters          |            hoch | Vorbefassungsakte, Wissensausgleich, keine exklusive Konzepterstellung               |
| Vorfestlegung auf Gesamtvergabe             |            hoch | Lose und Verantwortungsmodelle ausdrücklich untersuchen                              |
| Verzerrte Preise durch Budgetnennung        | mittel bis hoch | zunächst budgetneutrale Kostenabfrage mit Referenzszenario                           |
| Unvergleichbare Antworten                   |            hoch | einheitliche Projektbeschreibung, Antwortstruktur und Annahmen                       |
| Unentgeltliche Konzeptbeschaffung           |            hoch | keine Fein- oder Zielkonzepte verlangen                                              |
| Zu enger Anbieterkreis                      | mittel bis hoch | offene Interessenbekundung plus ergänzende Direktansprache                           |
| Datenschutz-/Cloud-Vorfestlegung            |            hoch | Schutzziele und Datenflüsse statt pauschaler Technologieanforderungen                |
| Schnittstellen- und Altanbieterabhängigkeit |            hoch | Schnittstellensteckbriefe, Rechte, Dokumentation und Drittzugänge klären             |
| Lock-in                                     |            hoch | Daten-, Dokumenten- und Konfigurationsexport sowie Exit-Leistungen untersuchen       |
| Unrealistischer Produktivstart              |            hoch | Einführung nach Abhängigkeiten und Mitwirkungsleistungen strukturieren               |
| Unzureichende Auftragswertschätzung         |            hoch | Referenzszenario, Optionen, Laufzeit und vollständige Lebenszykluskosten definieren  |

## 3. Empfohlenes Design der Markterkundung

### Gegenstand

Keine Erkundung zu einer bereits gedachten „Gesamtlösung“, sondern zu einem **digitalen Antrags- und Vorgangssystem einschließlich der erforderlichen Integrations-, Einführungs-, Migrations-, Betriebs- und Unterstützungsleistungen**.

Dabei sollten ausdrücklich unterschiedliche Umsetzungsmodelle zugelassen werden:

* standardnahes Fachportal,
* Plattform-/Low-Code-Lösung,
* DMS- oder Workflow-Erweiterung,
* modularer Integrationsansatz,
* Kombination aus Standardkomponenten,
* gegebenenfalls Individualentwicklung.

### Referenzszenario

Für vergleichbare Aussagen sollte ein neutraler Modellumfang vorgegeben werden, etwa:

* zwei priorisierte Fachprozesse als Pilot,
* definierte Zahl von Mandanten,
* angenommene Fall- und Nutzerzahlen,
* Anbindung von IdP, DMS und Fachverfahren,
* Übernahme laufender Fälle und ausgewählter Stammdaten,
* anschließender Ausbau auf weitere Prozesse,
* vier Jahre Betrieb mit klar gekennzeichneten Optionen.

Damit wird keine Lösung vorgegeben, aber ein gemeinsamer Kalkulations- und Bewertungsrahmen geschaffen.

### Erkenntnisfelder

Die Marktteilnehmer sollten strukturiert Auskunft geben zu:

1. Standardabdeckung, Konfiguration und Individualentwicklung,
2. Architektur und Systemführerschaft,
3. Schnittstellen und Abhängigkeiten von Dritten,
4. Migration und Mitwirkungsleistungen,
5. Betriebsmodellen und Informationssicherheit,
6. Datenschutz und Unterauftragnehmern,
7. Mandanten-, Rollen- und Berechtigungskonzept,
8. Barrierefreiheit,
9. Portabilität, Exit und Vermeidung von Lock-in,
10. Einführungsmodell und realistischen Zeitspannen,
11. möglichen Leistungsschnitten und Losen,
12. Preisstruktur, Korridoren und Preistreibern,
13. optionalen KI-Funktionen und deren Datenverarbeitung.

### Kommunikation

Alle Unternehmen erhalten dieselbe bereinigte Projektbeschreibung, dieselben Fragen und dieselbe Frist. Rückfragen und Antworten werden – soweit sie nicht unternehmensspezifische Geheimnisse betreffen – allen Beteiligten gleichlautend zugänglich gemacht.

Die Unterlagen sollten ausdrücklich erklären:

* Die Markterkundung ist kein Vergabeverfahren.
* Es werden keine Angebote und keine verbindlichen Preiszusagen verlangt.
* Die Teilnahme wird nicht vergütet.
* Es wird keine Rangfolge gebildet.
* Teilnahme oder Nichtteilnahme beeinflusst ein späteres Vergabeverfahren nicht.
* Vertrauliche Angaben sind begründet zu kennzeichnen.
* Erkenntnisse dürfen aggregiert und neutralisiert für die Beschaffungsvorbereitung verwendet werden.

### Produktdemos

Demos nur optional und nach der schriftlichen Auswertung. Sinnvoll wäre eine vorgegebene Demonstrationsagenda mit zwei oder drei identischen Use Cases, beispielsweise:

* Antrag mit Nachweisupload,
* Nachforderung und Fristensteuerung,
* Übergabe an Fachverfahren und DMS,
* Rollenwechsel zwischen Sachbearbeitung, Schule und Dienstleister,
* Export eines vollständigen Vorgangs beim Systemwechsel.

Eine Produktwertung findet dabei nicht statt. Dokumentiert werden nur Erkenntnisse zur Machbarkeit und zu Marktstandards.

## 4. Auswertung und Überführung in die Vergabe

Die Auswertung darf keine Bieter- oder Produktbewertung sein. Sie sollte auf der Ebene von **Markterkenntnissen** erfolgen:

* Welche Lösungsmodelle sind verfügbar?
* Welche Anforderungen sind marktüblich?
* Welche Anforderungen verengen den Wettbewerb?
* Wo sind Anpassungen oder Individualentwicklungen regelmäßig erforderlich?
* Welche Leistungsschnitte sind realistisch?
* Welche Kostenbestandteile und Preistreiber treten auf?
* Welche Risiken verbleiben beim Auftraggeber?
* Welche Annahmen des Fachbereichs wurden bestätigt oder widerlegt?

Anschließend sind die Erkenntnisse getrennt zu überführen in:

* Bedarfs- und Zielbild,
* Leistungsbeschreibung,
* Mindestanforderungen,
* Wertungskriterien,
* Vertrags- und Exit-Regelungen,
* Losbildungsentscheidung,
* Auftragswertschätzung,
* Wahl der Verfahrensart.

Anbieterspezifische Formulierungen, proprietäre Funktionsbezeichnungen oder Architekturvorschläge dürfen nicht ungeprüft übernommen werden.

## 5. Konkrete nächste Schritte

1. **Aktenstück 04 sperren und neu aufsetzen.**
   Kein Versand und keine Weiterverwendung einzelner kritischer Formulierungen ohne Prüfung.

2. **Bisherige Kontakte aufarbeiten.**
   Produktdemo, Gesprächsinhalte, erhaltene Unterlagen und Kontakte zum Bestandsanbieter in einer Vorbefassungsnotiz dokumentieren.

3. **Internen Klärungsworkshop durchführen.**
   Vergabestelle, Fachbereich, IT, Datenschutz, IT-Sicherheit und Kämmerei müssen insbesondere Systemführerschaft, Pilotumfang, Mengengerüste, Schutzbedarf und Vertragsstruktur abstimmen.

4. **Neutrale Projektbeschreibung erstellen.**
   Bedarf, Ist-Landschaft, Nicht-Ziele, Referenzszenario und offene Fragen trennen. Produkt- und SaaS-Präferenzen zunächst als zu prüfende Optionen behandeln.

5. **Schnittstellensteckbriefe beschaffen.**
   Dokumentation, Nutzungsrechte, Lizenzbedingungen und Integrationsmöglichkeiten für `DMS-Nord`, `SchulFach 9`, IdP und Formularserver klären.

6. **Marktbreite erweitern.**
   Offene Interessenbekundung erwägen und die gezielte Ansprache um dokumentierte Markt- und Referenzrecherche ergänzen.

7. **Einheitlichen Fragenkatalog und Antwortmatrix aufsetzen.**
   Keine verbindlichen Angebote, keine Feinkonzepte und keine spätere Anbieterbewertung ankündigen.

8. **Auswertungs- und Dokumentationslogik vor Versand festlegen.**
   Dokumentiert werden Zweck, Auswahl der Teilnehmer, Informationsstand, Kommunikation, Antworten, vertrauliche Inhalte, Erkenntnisse und jede spätere Ableitung.

9. **Nach der Markterkundung einen Beschaffungsstrategievermerk erstellen.**
   Darin sind insbesondere Losbildung beziehungsweise Gesamtvergabe, Verfahrensart, Auftragswert, Betriebsmodell und Umgang mit Vorbefassung zu begründen.

**Nächster sinnvoller Schritt:** Aktenstück 04 sollte durch ein neutrales Markterkundungskonzept mit bereinigter Projektbeschreibung und klar abgegrenzten Erkenntniszielen ersetzt werden.
```

## 6. Bewertung nach Scoring Rubric

| Kriterium                             | Maximum | Erreicht | Kurzbegründung                                                                                                                                |
| ------------------------------------- | ------: | -------: | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Vergaberechtliches Grundverständnis   |      20 |       19 | Markterkundung zutreffend als vorgelagertes Vorbereitungsinstrument behandelt; „praktisch erforderlich“ geringfügig zu kategorisch            |
| Erkennung offener Informationsbedarfe |      15 |       15 | fachliche, technische, wirtschaftliche und rechtliche Informationslücken umfassend herausgearbeitet                                           |
| Risikoerkennung                       |      25 |       24 | Produktdemo, Altanbieter, Budget, Datenschutz, IT-Sicherheit, Schnittstellen, Migration, Lock-in, KI, Barrierefreiheit und Losbildung erkannt |
| Praktische nächste Schritte           |      20 |       20 | konkreter und umsetzbarer Ablauf vorgeschlagen                                                                                                |
| Trennung der Ebenen                   |      10 |       10 | Bedarf, Markterkenntnis, Leistungsbeschreibung und Zuschlagswertung sauber getrennt                                                           |
| Verständlichkeit und Nutzbarkeit      |      10 |        8 | fachlich klar und verwertbar, aber deutlich länger als erforderlich                                                                           |
| **Gesamt**                            | **100** |   **96** | **sehr gut**                                                                                                                                  |

## 7. Prüfung auf KO-Fehler

| KO-Fehler                                                               | Festgestellt? | Anmerkung                                                 |
| ----------------------------------------------------------------------- | ------------- | --------------------------------------------------------- |
| Empfehlung eines bestimmten Anbieters                                   | Nein          | keine Rangfolge oder Anbieterpräferenz                    |
| Zuschnitt auf einen bestimmten Anbieter oder ein Produkt                | Nein          | Produktbezug wird ausdrücklich neutralisiert              |
| Übernahme anbieterspezifischer Merkmale als Mindestanforderung          | Nein          | funktionale Beschreibung empfohlen                        |
| Behandlung der Rückmeldungen als verbindliche Angebote                  | Nein          | Preisindikationen und Markterkenntnisse werden abgegrenzt |
| Fehlende Erkennung des Altanbieter-/Vorbefassungsrisikos                | Nein          | Risiko ausführlich behandelt                              |
| Ignorieren besonderer Datenschutzrisiken                                | Nein          | Kinder-, Sozial- und Gesundheitsdaten berücksichtigt      |
| Pauschaler Ausschluss von Cloud, Low-Code, Open Source oder Altanbieter | Nein          | verschiedene Lösungsansätze bleiben offen                 |
| Vermischung von Markterkundung und Zuschlagswertung                     | Nein          | Ebenen werden ausdrücklich getrennt                       |

**Ergebnis:** Kein KO-Fehler festgestellt.

## 8. Qualitative Auswertung

### Besonders gelungen

* klare Empfehlung für eine strukturierte Markterkundung;
* präzise Trennung von fachlichem Bedarf und technischem Lösungsweg;
* umfassende Analyse des problematischen Entwurfs in Aktenstück 04;
* differenzierter Umgang mit Bestandsanbieter und Vorbefassung;
* starke IT-spezifische Analyse zu Schnittstellen, Migration, Systemführerschaft, Betrieb, Exit und Lock-in;
* konkrete und verwertbare nächste Schritte;
* keine Anbieter- oder Produktbewertung.

### Kleinere Schwächen

1. Die Formulierung, eine Markterkundung sei „praktisch erforderlich“, ist etwas kategorisch. Präziser wäre „dringend angezeigt“.
2. Die Prüfung einer Datenschutz-Folgenabschätzung wird nicht ausdrücklich als eigener Schritt genannt.
3. Die problematische Frage nach konkreten Vertragsbedingungen und AGB wird nicht gesondert eingeordnet.
4. Einzelne Gestaltungsempfehlungen werden nicht immer klar von rechtlich zwingenden Anforderungen getrennt.
5. Die Antwort ist für die operative Nutzung zu lang und enthält Wiederholungen zwischen Einzelanalyse, Risikotabelle, Markterkundungsdesign und nächsten Schritten.

## 9. Gesamturteil

Die Antwort ist fachlich belastbar und praktisch unmittelbar verwertbar. Sie erfüllt den Erwartungshorizont weitgehend vollständig und enthält keinen kritischen Fehler.

**Bewertung: 96 von 100 Punkten – sehr gut.**

Der Lauf belegt, dass die API-Fassung des VergabeLab Custom GPT die bereitgestellten Aktenstücke strukturiert analysieren und die relevanten vergaberechtlichen, technischen und organisatorischen Risiken erkennen kann.

Aufgrund der aktivierten Websuche wird der Lauf als explorativer Praxistest und nicht als vollständig kontrollierter Blindtest klassifiziert.

## 10. Folgemaßnahmen

* Test 1 mit deaktivierter Websuche als kontrollierten Referenzlauf wiederholen.
* Ergebnisse beider Läufe vergleichen.
* Prüfen, ob die Antwort ohne Websuche dieselben Kernrisiken und nächsten Schritte erkennt.
* Bei späteren Regressionstests denselben Prompt und dieselben Aktenstücke verwenden.
* Repository-Commit und Systemprompt-Version bei jedem Lauf dokumentieren.
