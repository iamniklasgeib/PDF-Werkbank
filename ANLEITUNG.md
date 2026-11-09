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

## Funktionen

- **Lesen (L):** Text markieren und mit Strg+C kopieren
- **Suchen (Strg+F):** Enter springt zum nächsten Treffer, Umschalt+Enter zum vorherigen
- **Umbenennen:** Auf den Dateinamen oben links klicken, den Namen ändern und mit Enter bestätigen. Beim nächsten **Speichern** wird die Datei umbenannt.
- **Speichern (Strg+S):** Überschreibt die geöffnete Datei. Beim ersten Mal fragt der Browser, ob die App die Datei ändern darf.
- **Speichern unter (Strg+Umschalt+S):** Speichert als neue Datei.
- **Drucken (Strg+P):** Druckt mit allen Änderungen, die du gemacht hast.
- **Senden:** Öffnet das Windows-Teilen-Fenster. Dort wählst du Outlook oder Mail aus, die PDF ist dann schon angehängt.
- **Schließen (X):** Schließt das Dokument. Auch die letzte Seite kann jetzt gelöscht werden.
- **Zoom:** Strg+Mausrad, oder die Lupen-Buttons in der Werkzeugleiste

## Updates

1. Lade die neuen Dateien im Repository hoch: **Add file → Upload files**. Vorhandene Dateien werden dabei ersetzt.
2. Warte ein bis zwei Minuten, dann die App schließen und wieder öffnen. Falls die alte Version erscheint, die App noch einmal schließen und öffnen.
3. **Damit Windows das neue PDF-Symbol übernimmt, muss die App einmal neu installiert werden:**
   - Edge: `edge://apps` öffnen, bei PDF-Werkbank auf **⋯ → Deinstallieren** klicken
   - Chrome: `chrome://apps` öffnen, Rechtsklick auf PDF-Werkbank → **Aus Chrome entfernen**
   - Danach die Seite erneut öffnen, **App installieren** wählen und Schritt 5 wiederholen.
   - Falls Windows weiterhin das alte Symbol zeigt, einmal ab- und wieder anmelden. Windows speichert Dateisymbole zwischen.
