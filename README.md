# karriere.looops.at

Stelleninserate von Looops als eigenständige Seiten im Looops-Look, veröffentlicht über GitHub Pages
und per iFrame auf karriere.SN.at eingebunden.

## Aufbau

- `index.html` – das aktuelle Inserat (Marketing & Kommunikation – D2C und B2B), eine Datei, kein Build nötig
- `CNAME` – Custom Domain `karriere.looops.at` für GitHub Pages
- `.nojekyll` – GitHub Pages liefert die Dateien unverändert aus

## Schriften

Es liegen bewusst **keine Schriftdateien** im Repo (Web-Lizenzen von Cardinal und Maison Neue verlangen
Schutz gegen Fremdzugriff, den GitHub Pages nicht bietet). Überschriften sind in Cardinal gesetzt und
als SVG-Pfade eingebettet (durch die Desktop-Lizenz gedeckt), der Fließtext läuft in der Systemschrift
(Helvetica Neue / Arial). Neue Überschriften entstehen im Hub mit dem Skript aus der Claude-Session,
nicht durch Einbinden der Schrift.

## Ändern

Texte direkt in `index.html` anpassen (GitHub-Editor oder Pull Request). Nach dem Mergen in `main`
ist die Änderung in etwa einer Minute live; SN zeigt automatisch die neue Fassung.
