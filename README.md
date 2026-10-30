# Discgolfové mapy by Kuba Kemr

Web: https://dgmaps.vercel.app/ – každá změna nahraná sem na GitHub se na Vercelu nasadí sama (do minuty).

## Struktura

- `index.html` – hlavní stránka se seznamem map
- `roztyly-2026/`, `smecno-2026/`, `konopiste-2026/`, `bechovice-2026/`, `veltrusy-2026/`, `asuan-2026/` – jednotlivé mapy PDGL 2026 (každá má vlastní `index.html`)
- `assets/` – náhledy map (`<mapa>-2026.jpg`), JPEG ke stažení (`pdgl-<č>-<místo>-2026-mapa.jpg`), koš na pozadí, ikona webu

## Jak přidat novou mapu

1. Vytvoř složku, např. `konopiste-2027/`, a nahraj do ní HTML mapy přejmenované na `index.html`
   (v configu mapy nastav `"back_link": {"href": "../", "label": "Všechny mapy"}`, ať má tlačítko zpět).
2. Do `assets/` nahraj náhled mapy (JPEG cca 780×648 px), např. `konopiste-2027.jpg`.
3. V `index.html` zkopíruj blok mezi komentáři `Jedna mapa = jeden blok` a `konec bloku mapy`,
   uprav odkaz (`href="konopiste-2027/"`), obrázek, název, datum a údaje.
