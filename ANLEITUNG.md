# PDF-Werkbank als Standard-PDF-Öffner unter Windows

Dauer: etwa 10 Minuten. Du brauchst deinen GitHub-Account und Microsoft Edge oder Google Chrome.

## 1. Repository anlegen

1. Auf https://github.com einloggen.
2. Oben rechts auf **+** und dann **New repository** klicken.
3. Bei *Repository name* `pdf-werkbank` eintragen.
4. **Public** auswählen. GitHub Pages ist für private Repositorys nur mit einem Bezahl-Account möglich. Öffentlich ist nur der Programmcode, deine PDFs landen nie auf GitHub.
5. Auf **Create repository** klicken.

## 2. Dateien hochladen

1. Im neuen Repository auf den Link **uploading an existing file** klicken.
2. Die ZIP-Datei entpacken. Dann den **Inhalt** des Ordners `pdf-werkbank-app` in das Browserfenster ziehen: `index.html`, `manifest.json`, `sw.js` und die Ordner `lib` und `icons`.
   Wichtig: Die Datei `index.html` muss oben in der Liste stehen, nicht in einem Unterordner.
3. Unten auf **Commit changes** klicken.

## 3. GitHub Pages einschalten

1. Im Repository auf **Settings** gehen, dann links auf **Pages**.
2. Bei *Source* **Deploy from a branch** auswählen.
3. Bei *Branch* `main` und `/ (root)` auswählen und auf **Save** klicken.
4. Ein bis zwei Minuten warten. Die Adresse lautet dann
   `https://DEIN-BENUTZERNAME.github.io/pdf-werkbank/`
   (Sie erscheint auch oben auf der Pages-Einstellungsseite.)

## 4. Als App installieren

1. Die Adresse in **Edge** oder **Chrome** öffnen.
2. Dann installieren:
   - **Edge:** In der Adressleiste rechts auf das App-Symbol klicken, oder über **⋯ → Apps → Diese Website als App installieren**.
   - **Chrome:** In der Adressleiste rechts auf das Installieren-Symbol klicken, oder über **⋮ → Streamen, speichern und teilen → Seite als App installieren**.
3. Die PDF-Werkbank öffnet sich jetzt in einem eigenen Fenster. Sie steht im Startmenü und funktioniert ab jetzt auch offline.

## 5. Als Standard für PDFs einstellen

1. Mit der rechten Maustaste auf eine beliebige PDF klicken.
2. **Öffnen mit → Andere App auswählen** wählen.
3. **PDF-Werkbank** auswählen und auf **Immer** klicken.
   Falls sie nicht in der Liste steht: In den Windows-**Einstellungen → Apps → Standard-Apps** oben `.pdf` eingeben und dort PDF-Werkbank auswählen.
4. Beim ersten Doppelklick fragt der Browser eventuell, ob die PDF-Werkbank PDF-Dateien öffnen darf. Mit **Zulassen** bestätigen.

Ab jetzt öffnet ein Doppelklick auf eine PDF direkt die PDF-Werkbank. Wenn du mehrere PDFs markierst und gemeinsam öffnest, werden sie zu einem Dokument zusammengefügt.

## Speichern

**Speichern** öffnet einen normalen Windows-Speicherdialog. Dort kannst du einen Ort und einen Namen wählen. Vorgeschlagen wird `<Name>-bearbeitet.pdf`.

## Updates

Wenn du eine neue Version der Dateien hochlädst, erhöhe in `sw.js` die Zeile `const VERSION = 'v1';` (zum Beispiel auf `'v2'`). Danach die App einmal schließen und wieder öffnen.
