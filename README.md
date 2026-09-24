# Mystic Shop — Shulker-Bestellungen

Statische Bestell-Website (nur `index.html`, Tailwind via CDN, kein Build, kein Backend).

- Shulkerweise bestellen: Eisenbarren, Shulkerschalen, Blaze Rods, Pfeile, Knochen, Mohn (Poppies), Goldbarren, Goldnuggets, verrottetes Fleisch + leere Shulkerboxen pro Stück
- Preise nach `mysticItemDB / docs/data/worth.json` (Stand 24.09.2026), 1 volle Shulker = 1.728 Items
- Bestellung geht per FormSubmit an `lokrogamer.29@gmail.com`, Spieler erhält Bestellcode (`MV-XXXXXX`) für `/msg Lokrogamer CODE` ingame

## Lokal testen

```bash
cd mystic-shop
python -m http.server 8000
```

→ http://localhost:8000

## GitHub Pages

Deploy: Branch `main`, Root (`/`). `.nojekyll` liegt bei.
