---
title: "Testakte M-IT-01 – Ausgefüllter Bedarfserhebungsbogen Fachbereich"
version: "0.1.0"
last_reviewed: "2026-06-11"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "need-assessment"
eval_case_id: "M-IT-01"
eval_role: "input"
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

# Aktenstück 03 – Ausgefüllter Bedarfserhebungsbogen Fachbereich

## 1. Dokumentenstatus

**Dokumentart:** Interner Bedarfserhebungsbogen
**Ausgefüllt durch:** Fachbereich "Bildung und Teilhabe"
**Stand:** T0
**Zeitliche Einordnung:** Eingang des ausgefüllten Bedarfserhebungsbogens beim zentralen Vergabe-/Beschaffungsteam  
**Bearbeitungsstatus:** fachlich vorbefüllt, noch nicht durch Vergabestelle, IT und Datenschutz final geprüft

Dieser Bedarfserhebungsbogen wurde vom Fachbereich als Grundlage für die weitere Abstimmung mit IT, Datenschutz, Kämmerei und Vergabestelle erstellt. Er enthält fachliche Einschätzungen, erste Anforderungen und einzelne Formulierungen, die noch vergaberechtlich, technisch und datenschutzrechtlich zu prüfen sind.

## 2. Anlass und Problem

Die derzeitige Bearbeitung schulbezogener Verwaltungsleistungen ist aus Sicht des Fachbereichs nicht mehr ausreichend wirtschaftlich und bürgerfreundlich. Anträge gehen über unterschiedliche Kanäle ein, Nachweise werden mehrfach angefordert, Bearbeitungsstände sind für Antragstellende nicht transparent und Rückfragen erfolgen überwiegend per E-Mail oder Telefon.

Besonders aufwendig sind derzeit:

* manuelle Prüfung eingereichter Nachweise;
* Zuordnung von E-Mails zu laufenden Vorgängen;
* Rückfragen an Schulen und externe Dienstleister;
* Fristenkontrolle bei unvollständigen Anträgen;
* Übernahme von Daten in das Fachverfahren `SchulFach 9`;
* Ablage von Unterlagen im DMS;
* Erstellung von Bescheiden und Standardschreiben;
* Auswertungen für Teamleitung und Kämmerei.

Der Fachbereich erwartet, dass ein digitales Portal die Antragstellung vereinfacht und die interne Bearbeitung deutlich beschleunigt.

## 3. Betroffene Leistungen und geschätzte Fallzahlen

| Leistung                                   |      Geschätzte Fallzahl pro Jahr | Bemerkung                                        |
| ------------------------------------------ | --------------------------------: | ------------------------------------------------ |
| Schülerbeförderung / Fahrtkostenerstattung |                ca. 12.000 Anträge | saisonale Spitze vor Schuljahresbeginn           |
| Lernmittelfreiheit                         |                 ca. 8.500 Anträge | viele Nachweise zu Einkommen oder Leistungsbezug |
| Mittagsverpflegung / Zuschüsse             |                 ca. 6.000 Anträge | hoher Anteil unvollständiger Unterlagen          |
| Leihgeräteverwaltung                       |                ca. 3.500 Vorgänge | Ausgabe, Rückgabe, Verlust, Defekt               |
| Härtefall- und Einzelfallprüfungen         |                  ca. 900 Vorgänge | hoher Prüfaufwand, sensible Daten                |
| Rückfragen / Nachforderungen               | ca. 18.000 Kommunikationsvorgänge | über E-Mail, Telefon, Papier                     |

Die Fallzahlen beruhen auf Schätzungen des Fachbereichs. Eine belastbare Auswertung aus den bestehenden Systemen liegt bislang nicht vor.

## 4. Zielbild des Fachbereichs

Der Fachbereich wünscht sich eine Lösung, mit der Sorgeberechtigte und volljährige Schüler:innen Anträge online stellen, Nachweise hochladen und den Bearbeitungsstand einsehen können. Schulen und externe Dienstleister sollen bei Bedarf eingebunden werden, ohne Zugriff auf nicht erforderliche Daten zu erhalten.

Aus Sicht des Fachbereichs sollte die Lösung möglichst viele Standardprozesse bereits enthalten. Eine Lösung, die erst vollständig konfiguriert oder individuell entwickelt werden muss, wird als risikoreich eingeschätzt, weil der Fachbereich dafür keine ausreichenden Kapazitäten hat.

Gewünscht wird insbesondere:

* ein einheitliches Portal für alle genannten Leistungen;
* vorkonfigurierte Antragsstrecken für schulbezogene Leistungen;
* digitale Nachforderung fehlender Unterlagen;
* automatische Erinnerung bei Fristablauf;
* Rollen- und Rechtekonzept für Sachbearbeitung, Schulen und Dienstleister;
* Übergabe relevanter Daten an `SchulFach 9` und DMS;
* Bescheidvorbereitung auf Basis geprüfter Daten;
* Auswertungen zu Eingang, Bearbeitungsdauer, Rückständen und Fristen;
* möglichst einfache Erweiterbarkeit auf weitere Leistungen.

## 5. Vorläufige Anforderungen aus Sicht des Fachbereichs

Die folgende Liste ist eine fachliche Erstsammlung. Sie ist noch nicht als Leistungsbeschreibung zu verstehen.

| Priorität | Anforderung / Wunsch                                                    | Bemerkung Fachbereich                                  |
| --------- | ----------------------------------------------------------------------- | ------------------------------------------------------ |
| Muss      | Online-Antragstellung mit Upload von Nachweisen                         | mobile Nutzung wichtig                                 |
| Muss      | Statusanzeige für Antragstellende                                       | reduziert Rückfragen                                   |
| Muss      | Rollen- und Rechtekonzept                                               | verschiedene Kommunen und Schulen                      |
| Muss      | Mehrmandantenfähigkeit                                                  | mehrere Trägerkommunen müssen getrennt abbildbar sein  |
| Muss      | Schnittstelle oder Export zu `SchulFach 9`                              | derzeit mindestens CSV erforderlich                    |
| Muss      | Ablage im DMS                                                           | möglichst automatisch                                  |
| Muss      | deutsche Benutzeroberfläche                                             | auch für Support erforderlich                          |
| Soll      | vorkonfigurierte Prozesse für Schülerbeförderung und Lernmittelfreiheit | Fachbereich möchte keinen kompletten Neubau            |
| Soll      | integrierte Vorlagen für Rückfragen und Bescheide                       | rechtliche Prüfung bleibt intern                       |
| Soll      | Erinnerungs- und Fristenfunktionen                                      | insbesondere vor Schuljahresbeginn                     |
| Soll      | Auswertungen und Dashboards                                             | für Teamleitung und Kämmerei                           |
| Soll      | Betrieb als SaaS aus EU-Rechenzentren                                   | Fachbereich bevorzugt geringe interne Betriebsaufwände |
| Wunsch    | KI-gestützte Dokumentenklassifikation                                   | z. B. Nachweise automatisch erkennen                   |
| Wunsch    | Textvorschläge für Rückfragen                                           | keine automatische Entscheidung                        |
| Wunsch    | Chatbot für häufige Fragen                                              | nur allgemeine Hinweise, keine Rechtsberatung          |
| Wunsch    | sehr kurze Einführungszeit                                              | produktiver Pilot frühestens ab T+12 Monate                       |

## 6. Vom Fachbereich gewünschte Eigenschaften der Lösung

Der Fachbereich hält folgende Eigenschaften für besonders wichtig:

* Die Lösung soll möglichst „aus einer Hand“ bereitgestellt werden.
* Die Lösung soll bereits bei anderen Kommunen im Schulbereich im Einsatz sein.
* Die Lösung soll ohne umfangreiche interne Entwicklungsarbeit produktiv nutzbar sein.
* Die Lösung soll eine moderne Oberfläche haben und auch auf Smartphones gut funktionieren.
* Die Lösung soll einfache fachliche Änderungen, etwa an Formularen, Textbausteinen, Fristen oder Prozessschritten, durch geschulte Mitarbeitende konfigurierbar machen, ohne dass hierfür stets eine Individualentwicklung erforderlich ist.
* Die Lösung soll Datenexporte ermöglichen, falls später ein Systemwechsel erforderlich wird.
* Die Lösung soll möglichst wenig zusätzliche IT-Betriebsverantwortung bei der AöR auslösen.

Der Fachbereich weist darauf hin, dass eine im T-6 Wochen vorgestellte Produktlösung eines Marktteilnehmers viele dieser Punkte bereits abbilden soll. Eine technische und rechtliche Prüfung dieser Angaben hat noch nicht stattgefunden.

## 7. Bestehende fachliche Unsicherheiten

Aus Sicht des Fachbereichs sind insbesondere folgende Punkte unklar:

1. Ob es marktverfügbare Lösungen gibt, die mehrere der genannten Leistungen standardnah abdecken.
2. Ob eine Low-Code-Plattform für die Fachprozesse ausreicht oder zu viel Eigenaufwand erzeugt.
3. Ob bestehende DMS- und Fachverfahrensschnittstellen ohne Individualentwicklung angebunden werden können.
4. Ob eine SaaS-Lösung bei den verarbeiteten Datenarten datenschutzrechtlich und organisatorisch tragfähig ist.
5. Welche Daten aus Altsystemen migriert werden müssen und welche Altakten lediglich recherchierbar bleiben sollen.
6. Ob Schulen und externe Dienstleister eigene Portalkonten erhalten sollten oder ob ein anderer Datenaustausch ausreicht.
7. Welche Anforderungen an Barrierefreiheit, mobile Nutzung und Mehrsprachigkeit realistisch sind.
8. Welche KI-Funktionen am Markt verfügbar sind und welche davon für den Fachbereich überhaupt sinnvoll wären.

## 8. Datenschutz und besondere Schutzbedarfe

Der Fachbereich geht davon aus, dass in der Lösung personenbezogene Daten von Kindern, Sorgeberechtigten und Haushalten verarbeitet werden. In einzelnen Fällen können auch sensible Angaben betroffen sein, etwa bei Härtefällen, besonderem Beförderungsbedarf oder Leistungsnachweisen.

Folgende Punkte sind aus Sicht des Fachbereichs wichtig, aber noch nicht abschließend geklärt:

* Welche Daten dürfen Schulen sehen?
* Welche Daten dürfen externe Dienstleister sehen?
* Wie lange müssen Unterlagen im Portal verfügbar sein?
* Welche Unterlagen müssen in die E-Akte oder das DMS übernommen werden?
* Wie sollen Lösch- und Aufbewahrungsfristen umgesetzt werden?
* Welche Protokollierung ist erforderlich?
* Ob eine Datenschutz-Folgenabschätzung erforderlich wird.

Der Fachbereich möchte vermeiden, dass Datenschutzanforderungen erst nach Auswahl einer Lösung geklärt werden.

## 9. Betrieb, Support und Schulung

Der Fachbereich verfügt nicht über eigene technische Betriebskapazitäten. Gewünscht wird daher ein Betriebsmodell, bei dem Wartung, Updates, Hosting und technischer Support weitgehend durch den Auftragnehmer oder einen Dienstleister erbracht werden.

Offen ist, ob der Betrieb erfolgen sollte als:

* SaaS aus einem EU-Rechenzentrum;
* Private-Cloud-Betrieb;
* Betrieb im kommunalen Rechenzentrum;
* On-Premises-Betrieb bei der AöR.

Für die Einführung werden Schulungen für Sachbearbeitung, Teamleitung und IT-Administration benötigt. Zusätzlich werden kurze Anleitungen für Schulen und externe Dienstleister benötigt. Der Fachbereich wünscht sich eine möglichst einfache Konfiguration ohne dauerhafte Abhängigkeit vom Auftragnehmer.

## 10. Migration und Übergang

Der Fachbereich hält eine vollständige Migration sämtlicher historischer Akten nicht für zwingend erforderlich. Wichtig ist aber, dass laufende Anträge und relevante Stammdaten zum Produktivstart übernommen oder zumindest in geordneter Form verfügbar sind.

Offene Punkte:

* Welche Daten aus `SchulFach 9` müssen initial übernommen werden?
* Welche Dokumente aus dem DMS müssen mit Vorgängen verknüpft werden?
* Ob alte PDF-Anträge nur recherchierbar bleiben oder in neue Vorgänge überführt werden sollen.
* Welche Mitwirkung der AöR bei Datenbereinigung, Testmigration und Abnahme erforderlich ist.
* Wie lange ein Parallelbetrieb notwendig wäre.

Der Fachbereich geht zum Aktenstand davon aus, dass ein Produktivstart einer Pilotkommune innerhalb von sechs bis neun Monaten nach Zuschlag realistisch sein könnte. Diese Einschätzung ist nicht technisch validiert.

## 11. Budget und Wirtschaftlichkeit

Für Einführung, Migration, Schulung und Betrieb über vier Jahre wird zum Aktenstand ein Korridor von 850.000 EUR bis 1.400.000 EUR netto diskutiert. Der Fachbereich kann nicht einschätzen, ob dieser Korridor für die genannten Anforderungen realistisch ist.

Aus Sicht des Fachbereichs sollten in einer Markterkundung zumindest Größenordnungen zu folgenden Kostenbestandteilen erfragt werden:

* Einführung und Projektmanagement;
* Lizenz- oder Nutzungsentgelte;
* Hosting und Betrieb;
* Schnittstellen;
* Migration;
* Schulung;
* Support;
* optionale Module;
* spätere Erweiterungen.

Der Fachbereich möchte vermeiden, dass im Haushalt ein zu niedriger Ansatz angemeldet wird und das spätere Vergabeverfahren daran scheitert.

## 12. Bekannte Marktinformationen

Dem Fachbereich sind bislang folgende Marktinformationen bekannt:

* Eine Produktpräsentation eines Anbieters im T-6 Wochen hat gezeigt, dass es offenbar spezialisierte Fachportale für schulbezogene Verwaltungsleistungen gibt.
* Die IT-Abteilung hat darauf hingewiesen, dass auch Low-Code-Plattformen, DMS-/Workflow-Erweiterungen und Open-Source-nahe Integrationsansätze in Betracht kommen könnten.
* Der Bestandsanbieter des Fachverfahrens `SchulFach 9` hat informell angeboten, ohne gesonderte Vergütung ein Konzept für eine Portalmodernisierung zu erstellen. Eine vergaberechtliche und technische Einordnung dieses Angebots liegt noch nicht vor.
* Mehrere Nachbarkommunen nutzen nach Auskunft einzelner Mitarbeitender bereits digitale Antragsportale, Details zu Architektur, Vergabe und Betrieb liegen aber nicht vor.

Die Angaben sind bislang nicht systematisch geprüft und nicht dokumentiert.

## 13. Vom Fachbereich vorgeschlagene Fragen an den Markt

Der Fachbereich schlägt vor, in einer Markterkundung insbesondere folgende Fragen zu stellen:

1. Welche vergleichbaren Portallösungen haben Sie bereits für Kommunen umgesetzt?
2. Für welche schulbezogenen Verwaltungsprozesse bietet Ihre Lösung bereits Standardfunktionen an, etwa Antragstellung, Nachweisupload, Statusanzeige, Nachforderungen, Bescheidvorbereitung, Schnittstellen/Exporte oder Auswertungen?
3. Welche Anforderungen müssten individuell entwickelt werden?
4. Wie schnell könnten Sie eine Pilotkommune produktiv setzen?
5. Können Sie bestätigen, dass Ihre Lösung mit `DMS-Nord` und `SchulFach 9` funktioniert?
6. Können Sie eine verbindliche Preisindikation für vier Jahre abgeben?
7. Welche Vertragsbedingungen und AGB verwenden Sie üblicherweise?
8. Welche KI-Funktionen enthält Ihre Lösung?
9. Können Sie einen kostenfreien Workshop durchführen und danach ein Grobkonzept liefern?
10. Welche technischen Anforderungen sollten wir in die spätere Ausschreibung aufnehmen?

Diese Fragen sind fachlich vorformuliert und noch nicht durch die Vergabestelle freigegeben.

## 14. Vorläufige Einschätzung des Fachbereichs

Der Fachbereich sieht den größten Nutzen in einer Lösung, die möglichst viele Fachprozesse bereits mitbringt und wenig interne Konfigurationsarbeit erfordert. Eine reine Plattformlösung erscheint dem Fachbereich nur dann geeignet, wenn sie mit belastbaren Referenzen, geringem Einführungsaufwand und klarer Betriebsverantwortung verbunden ist.

Gleichzeitig ist dem Fachbereich bewusst, dass noch keine belastbare Marktübersicht besteht und dass die bisherigen Eindrücke vor allem auf Einzelgesprächen, einer Produktdemonstration und informellen Hinweisen beruhen.

Eine Markterkundung wird aus Sicht des Fachbereichs als sinnvoll angesehen, wenn sie zu einer besseren Einschätzung von Lösungsansätzen, Kosten, Umsetzungsaufwand, Betriebsmodellen und Risiken führt.
