# Tessa · Rekomposition

Tessas App für den 12-Wochen-Plan vom 29.10.2026 bis 24.01.2027: Training, Ernährung, Zyklus-Tracker, Readiness und Messungen in einer Oberfläche. Sie läuft komplett im Browser, funktioniert offline und speichert alle Einträge nur auf dem Handy.

---

## 1. Online stellen mit GitHub Pages

Einmalig, etwa zehn Minuten.

1. **Bei GitHub anmelden** auf github.com (oder kostenlos registrieren).
2. **Neues Repository anlegen:** oben rechts auf **+** und dann **New repository**.
   - Name zum Beispiel `tessa`.
   - Sichtbarkeit **Public**. Mit einem kostenlosen Konto gibt es GitHub Pages nur für öffentliche Repositories. Öffentlich ist dabei nur der Code der App, nicht Tessas Einträge — die liegen ausschließlich auf ihrem Handy.
   - Unten auf **Create repository** klicken.
3. **Dateien hochladen:** Auf der neuen, leeren Seite auf den Link **uploading an existing file** klicken. Den Ordner aus dem ZIP öffnen und **alles darin** ins Browserfenster ziehen, auch den Ordner `fonts`. Danach unten **Commit changes** klicken.
4. **Pages einschalten:** Im Repository oben auf **Settings**, links auf **Pages**. Unter *Build and deployment* bei *Source* **Deploy from a branch** wählen, darunter Branch **main** und Ordner **/ (root)**, dann **Save**.
5. **Ein bis zwei Minuten warten** und die Seite neu laden. Oben steht dann die Adresse, zum Beispiel `https://DEINNAME.github.io/tessa/`.

**Schon ein Repository für deine eigene App?** Dann kannst du Tessas App auch dort in einen eigenen Ordner legen, zum Beispiel `tessa/`. Die Adresse ist dann `https://DEINNAME.github.io/REPO/tessa/`. Eure Daten mischen sich nicht.

> Die Datei `.nojekyll` ist auf dem Mac unsichtbar. Wenn sie beim Hochladen fehlt, ist das kein Problem — die App funktioniert auch ohne.

---

## 2. Auf Tessas iPhone installieren

1. Die Adresse in **Safari** öffnen.
2. Unten auf das **Teilen-Symbol** tippen (Quadrat mit Pfeil nach oben).
3. **Zum Home-Bildschirm** wählen und **Hinzufügen** tippen.
4. Ab jetzt die App immer über das neue Symbol öffnen.

**Wichtig:** Die installierte App hat ihren eigenen Speicher, getrennt von Safari. Also immer über das Symbol eintragen, nicht mal so und mal so.

Beim ersten Öffnen fragt die App nach Verhütung, Zykluslänge, Periodendauer und letztem Periodenbeginn. Das lässt sich überspringen und später im Tab **Trends** unter **Zyklus** nachtragen.

---

## 3. Datensicherung

Alle Einträge liegen nur auf diesem einen Gerät. Deshalb:

- **Alle zwei Wochen** im Tab **Trends** ganz unten auf **Sicherung herunterladen** tippen und die Datei sichern, zum Beispiel in iCloud Drive.
- **Neues Handy oder App gelöscht?** App wie oben neu installieren, dann **Trends → Sicherung einspielen** und die Datei auswählen.

---

## 4. Eine neue Version einspielen

1. Im Repository auf **Add file → Upload files**, die neue `index.html` hineinziehen und **Commit changes** klicken. Die alte Datei wird dabei ersetzt.
2. Auf dem iPhone holt sich die App die neue Version beim nächsten Öffnen mit Internet. Falls nicht: App einmal ganz schließen (nach oben wischen) und neu öffnen.

Tessas Einträge bleiben dabei erhalten — sie liegen auf dem Handy, nicht im Repository.

---

## Was in dem Ordner steckt

| Datei | Wofür |
|---|---|
| `index.html` | die komplette App |
| `manifest.webmanifest` | Name und Symbol für den Home-Bildschirm |
| `sw.js` | sorgt dafür, dass die App auch ohne Internet startet |
| `*.png` | App-Symbole |
| `fonts/` | die beiden Schriften samt Lizenz (SIL Open Font License) |
| `.nojekyll` | sagt GitHub, die Dateien unverändert auszuliefern |

## Datenschutz

Die App schickt keine Daten irgendwohin und lädt nichts von fremden Servern — auch die Schriften liegen im Ordner. Zyklus, Gewicht und alle anderen Einträge bleiben im Speicher des Geräts.
