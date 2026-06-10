---
title: "Beitrag zur VergabeLab Community"
version: "0.1.1"
last_reviewed: "2026-06-10"
status: "initial"
language: "de-DE"
type: "policy"
license: "CC-BY-4.0"
repository_area: "root"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Community-Mitwirkende"
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Entwicklerinnen und Entwickler"
topics:
  - "Contributing"
  - "DCO"
  - "Inbound = Outbound"
  - "SPDX"
  - "YAML-Frontmatter"
  - "Pull Requests"
  - "Issues"
  - "Community-Beiträge"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# Beitrag zur VergabeLab Community (Contributing)

Vielen Dank für dein Interesse an VergabeLab Community. Beiträge sind ausdrücklich willkommen. Auch ohne „Git-Profi“ zu sein.

---

## 1) Grundprinzip: Inbound = Outbound

Beiträge werden unter der Lizenz des jeweiligen Ordners/der Datei veröffentlicht (siehe README „Lizenzierung“).  
Für Textartefakte ist das in der Regel **CC BY 4.0**, sofern in der Datei nicht anders gekennzeichnet.

**Kurz:** Wenn du einen Beitrag einreichst, erklärst du dich damit einverstanden, dass er unter der für den betroffenen Ordner/die Datei geltenden Lizenz veröffentlicht wird.

---
## 2) Pflicht: DCO (Developer Certificate of Origin)

Wir nutzen das **Developer Certificate of Origin (DCO)**, um sicherzustellen, dass Beiträge rechtlich sauber eingebracht werden können. Den genauen rechtlichen Wortlaut, dem du dabei zustimmst, findest du in unserer Datei [`DCO.md`](DCO.md).

### Was du tun musst
Jeder Commit in einem Pull Request muss ein `Signed-off-by` enthalten. Pull Requests **ohne** vollständige Sign-offs werden nicht gemergt; der GitHub-Statuscheck **`DCO / DCO sign-off check`** ist dafür verpflichtend.

**Beispiel:**
```text
Signed-off-by: Vorname Nachname <email@example.com>
```
**Datenschutzfreundlicher Hinweis:** Du musst hierfür nicht zwingend deine private E-Mail-Adresse verwenden. GitHub stellt eine `noreply`-Adresse bereit, die mit deinem Konto verknüpft ist. Du findest sie unter `Settings → Emails`, wenn du „Keep my email addresses private“ aktivierst. Der Signoff kann dann z. B. so aussehen:

```text
Signed-off-by: Vorname Nachname <ID+username@users.noreply.github.com>
```

### So signierst du Commits (Git)
**Einmalig pro Commit:**
```bash
git commit -s -m "Deine Beschreibung"
```
**Bei Beiträgen über die GitHub-Weboberfläche:** Da in diesem Repository die Option „Require contributors to sign off on web-based commits“ aktiviert ist, fügt GitHub den Signoff bei Web-Commits automatisch hinzu. Bitte prüfe dennoch, ob der DCO-Check erfolgreich durchläuft.

**Für bereits vorhandene Commits (Rewrite, mit Vorsicht):**
```bash
git commit --amend -s
git push --force-with-lease
```

**Wenn der DCO-Check fehlschlägt (typischer Fix):**
```bash
# letzten Commit nachsignieren
git commit --amend -s

# mehrere Commits nachsignieren
git rebase -i origin/main

# bei jedem "edit"
git commit --amend -s && git rebase --continue
```

**Kurz:** Mit dem Sign-off bestätigst du, dass du den Beitrag selbst erstellt hast oder die nötigen Rechte besitzt, ihn unter der jeweiligen Projektlizenz beizusteuern.

---

## 3) Was wir nicht annehmen (bitte beachten)

Damit VergabeLab öffentlich nutzbar bleibt:

* **Keine personenbezogenen Daten** (Namen, Kontaktdaten, Signaturen etc.)
* **Keine Details laufender Vergaben**
* **Keine Betriebs- und Geschäftsgeheimnisse**
* Bitte nur **abstrahierte/anonymisierte Beispiele** („Bieter A/B“, „Projekt X“, „Leistungskategorie Y“)
* Falls interne Freigaben erforderlich sind: bitte vor Veröffentlichung intern klären.

---

## 4) Wege, wie du beitragen kannst

### A) Issue (Diskussion & Ideen)
Nutze Issues für Feedback, Ideen, Bugs, rechtliche Updates oder Wünsche für neue Bausteine.

### B) Pull Request (konkrete Änderungen)
Pull Requests sind ideal für konkrete Verbesserungen an Prompts, Guides oder Templates.

### C) Pilot-Feedback (Erfahrungen aus der Praxis)
Erfahrungen aus realen Projekten sind besonders wertvoll (bitte anonymisiert).

---
## 5) SPDX-Header & Autorenschaft (Pflicht)

Bitte füge jeder neuen oder wesentlich geänderten Markdown-Datei am Anfang ein YAML-Frontmatter mit Metadaten und anschließend einen SPDX-Kommentar hinzu:

```text
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

Bei modulgebundenen Dateien ist zusätzlich die Modulzuordnung nach [POLICIES/SPDX.md](POLICIES/SPDX.md) zu beachten; insbesondere kann dort ein `module_id` erforderlich sein.

Grundsatz: Im Header steht der tatsächliche Rechteinhaber/Autor (bei Co-Authoring mehrere Zeilen). Durch das Einreichen eines Beitrags erfolgt keine automatische Rechteübertragung; es gelten die Nutzungsrechte nach der jeweiligen Lizenz in der Datei.

Details und Beispiele: siehe [`POLICIES/SPDX.md`](POLICIES/SPDX.md)

**Danke für deinen Beitrag!**
