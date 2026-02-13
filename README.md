# Valentine's Day — «Будешь моей Валентинкой?»

A small, playful Valentine's page: one question, compliments, flying photos, hearts, and confetti.

## What it does

- **Main question:** «Будешь моей Валентинкой?» with **Да** / **Нет**.
- **«Нет»** moves around; after a few hovers, a second **Да** appears and a «Нажми да» popup shows.
- **First «Да»:** Title becomes «Я тебя люблю, Буся», button turns into **Новый комплимент**, and photos start flying across the screen (from the `image/` folder).
- **Photos:** Loaded from `image/photos.json`; circles with pink borders fly in from all sides (including diagonals), in random order; same photo can appear 2–3 times.
- **Hearts:** Small hearts orbit each photo; background hearts float across the whole page.
- **«Новый комплимент»:** Shows a random compliment from a list, triggers a short scale “pulse” on all photos, then pink particle bursts around each photo and confetti around the card and images (no top-only spawn).

## Setup

1. Put your images in the `image/` folder.
2. List them in `image/photos.json` as an array of filenames, e.g.:
   ```json
   ["photo1.jpg", "photo2.jpg"]
   ```
3. Open `index.html` in a browser (or serve the folder with any static server, e.g. `python -m http.server 5500`).

## Tech

- Single HTML file: structure, styles, and script in `index.html`.
- No build step; no external dependencies.
