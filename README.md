# karriere.looops.at

Stelleninserate von Looops als eigenständige Seiten im Looops-Look, veröffentlicht über GitHub Pages
und per iFrame auf karriere.SN.at eingebunden.

## Aufbau

- `index.html` – Übersicht aller offenen Stellen
- `<slug>/index.html` + `hero.jpg` + `hero.webp` – je Stelle ein Ordner (`marketing-kommunikation/`, `vertrieb-partnerbetreuung/`)
- `CNAME` – Custom Domain `karriere.looops.at` für GitHub Pages
- `.nojekyll` – GitHub Pages liefert die Dateien unverändert aus

Quelle je Stelle ist `inserat-<slug>.json` im Looops Hub (`Marketing/Claude/Karriere - Stellenanzeigen/`);
gebaut wird mit dem Skript aus dem Skill `looops-stelleninserat`, nicht von Hand im HTML.

## Schriften

Es liegen bewusst **keine Schriftdateien** im Repo (Web-Lizenzen von Cardinal und Maison Neue verlangen
Schutz gegen Fremdzugriff, den GitHub Pages nicht bietet). Überschriften sind in Cardinal gesetzt und
als SVG-Pfade eingebettet (durch die Desktop-Lizenz gedeckt), der Fließtext läuft in der Systemschrift
(Helvetica Neue / Arial).

## Ändern

JSON im Hub anpassen, neu bauen, geänderte Dateien hochladen. Nach dem Commit in `main`
ist die Änderung in etwa einer Minute live; SN zeigt automatisch die neue Fassung.
Stelle besetzt: Ordner löschen, Übersicht neu bauen und hochladen, bei SN deaktivieren.
