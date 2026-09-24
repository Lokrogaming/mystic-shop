# Mystic Shop — Shulker-Bestellungen

Statische Bestell-Website (nur `index.html`, Tailwind via CDN, kein Build, kein Backend).

- Shulkerweise bestellen: Eisenbarren, Shulkerschalen, Blaze Rods, Pfeile, Knochen, Mohn (Poppies), Goldbarren, Goldnuggets, verrottetes Fleisch + leere Shulkerboxen pro Stück
- Preise werden live per HTTP aus `mysticItemDB / docs/data/worth.json` geladen (eingebettete Fallback-Preise), 1 volle Shulker = 1.728 Items
- Anzeigen netto, Checkout: Zwischensumme + 15 % Zahlungsgebühr = zahlbarer Gesamtbetrag
- Bestellung geht per FormSubmit an `lokrogamer.29@gmail.com` **und** parallel als Zeile ins Google Sheet (Google-Formular, kein API-Key), Spieler erhält Bestellcode (`MV-XXXXXX`) für `/msg Lokrogamer CODE` ingame

## Lokal testen

```bash
cd mystic-shop
python -m http.server 8000
```

→ http://localhost:8000

## GitHub Pages

Deploy: Branch `main`, Root (`/`). `.nojekyll` liegt bei.
