# theo-gottschalch.github.io

"Im Aufbau"-Seite für die kommende Naturfotografie-Website.

- `index.html` — Inhalt der Seite
- `style.css` — Gestaltung (helles Papierweiß, Serif-Typografie, keine externen Abhängigkeiten)
- `images/` — drei Bilder, auf 1400 px Breite verkleinert
- `.nojekyll` — verhindert die Jekyll-Verarbeitung auf GitHub Pages

## Veröffentlichen

Dateien auf den Standardbranch pushen, dann in den Repository-Einstellungen unter
**Settings → Pages** als Quelle *Deploy from a branch* → `main` / `/ (root)` wählen.
Die Seite ist danach unter <https://theo-gottschalch.github.io> erreichbar.

## Bilder austauschen

Verkleinerte Fassung erzeugen und in `images/` legen, danach `src` und `alt`
in `index.html` anpassen:

```bash
sips -Z 1400 -s format jpeg -s formatOptions 72 original.jpg --out images/neu.jpg
```
