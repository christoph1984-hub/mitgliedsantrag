# Mitgliedsantrag

Digitale Mitgliedsanträge für KulturOase e.V. und Streuobstwiesenfreunde e.V.
Interessierte füllen das Formular aus, unterschreiben am Bildschirm und laden ein PDF herunter, das sie an die Vereins-E-Mail schicken.

| Verein | Link |
|---|---|
| KulturOase e.V. | https://christoph1984-hub.github.io/mitgliedsantrag/kulturoase/ |
| Streuobstwiesenfreunde e.V. | https://christoph1984-hub.github.io/mitgliedsantrag/streuobstwiesenfreunde/ |

## Wichtig

- Dieses Repo enthält nur die leeren Formulare. **Ausgefüllte Anträge nie hier hochladen**, sie gehören in den Vereinsordner.
- Die Seite überträgt keine Daten. Das PDF entsteht im Browser der Person, die den Antrag ausfüllt.
- Keine externen Dienste (keine Google Fonts, kein CDN). Die PDF-Bibliothek liegt in `assets/` (jsPDF 2.5.1, MIT-Lizenz).

## Inhalte ändern

Alle Vereinsangaben (Adresse, E-Mail, IBAN, Beitrag, Mitmach-Bereiche, Vorstand) stehen oben im Skript der jeweiligen `index.html` im Block `const VEREINE = { … }`.
Auf github.com die Datei öffnen, Stift-Symbol, ändern, „Commit changes“. Nach ein bis zwei Minuten ist die Änderung online.

- `glaeubigerId` bleibt leer, solange keine Lastschrift angeboten werden soll.
- Für einen weiteren Verein: Ordner `kulturoase/` kopieren, umbenennen, Angaben im Block `VEREINE` und im Aufruf `form("…")` am Ende anpassen.

## Ordner

```
index.html                    Hinweisseite ohne Vereinsauswahl
kulturoase/index.html         Formular KulturOase e.V.
streuobstwiesenfreunde/index.html  Formular Streuobstwiesenfreunde e.V.
assets/jspdf.umd.min.js       PDF-Erzeugung im Browser
```
