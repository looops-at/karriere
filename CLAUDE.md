# CLAUDE.md – karriere.looops.at

Dieses Repo trägt die Stelleninserate auf karriere.looops.at (GitHub Pages, per iFrame auf karriere.SN.at).
Gebaut und gepflegt wird es mit dem Skill `looops-stelleninserat` – dort stehen Ablauf und Gestaltungsregeln.

## Regeln für dieses Repo

- **Direkt auf `main`** committen und pushen ist hier erlaubt, sobald die Vorschau freigegeben ist. Branch und PR nur, wenn noch jemand drüberschauen soll.
- **Nicht von Hand im HTML ändern.** Quelle ist `inserat-<slug>.json` im Hub (`Marketing/Claude/Karriere - Stellenanzeigen/`), danach neu bauen.
- **Keine Schriftdateien** (`otf`, `woff`, `woff2`) und keine Links aufs Shop-CDN.
- **Kein Token** aus dem Chat verwenden oder danach fragen.
- `CNAME` und `.nojekyll` bleiben unangetastet.
- Alles in diesem Repo ist öffentlich abrufbar, auch diese Datei.

## ⚠️ Diese lockeren Regeln gelten nur hier

Die Shop-Themes haben strengere Regeln, auch wenn sie im selben Auftrag mitgeändert werden:

| Repo | Regeln |
|---|---|
| `looops-at/karriere` (dieses) | direkt auf `main` ok |
| `looops-at/d2c-stretch` (looopsmoments.com, z. B. `/pages/job-…`) | nie auf `main`/`develop`; `fix/*`- oder `content/*`-Branch von `develop`, PR nach `develop`, Merge nur durch Julia oder Luisa |
| `looops-at/b2b-stretch` (partner.looops.at) | wie D2C |

Nie `shopify theme push` oder `--live` – Änderungen am Live-Theme laufen immer über das Theme-Repo.
In `d2c-stretch` schreibt Claude nur mit ausdrücklichem OK; sonst geht die Änderung an Luisa.
Vor Arbeit an einem Theme-Repo dessen `CLAUDE.md` lesen.
