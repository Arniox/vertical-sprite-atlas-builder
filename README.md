# Sprite Atlas Builder

A tiny browser-only sprite strip atlas builder that is ready for GitHub Pages.

[Sprite Atlas Builder](https://arniox.github.io/vertical-sprite-atlas-builder/)

## What it does

- Drag/drop unlimited sprite strips or sheets.
- Reorder strips with drag/drop or buttons.
- Auto-clear common fake checkerboard backgrounds.
- Debounced checker cleanup tolerance.
- Blur/loading overlay while the preview is rebuilding.
- Optional transparent-edge trimming.
- Optional strip height/width normalization.
- Per-strip scale and nudge controls.
- Final padding between strips after cleanup, trimming, normalization, scaling, and alignment.
- Export normal PNG/WebP atlases.
- Export a Codex pet package containing:
  - `pet.json`
  - `spritesheet.webp`

## GitHub Pages setup

This repo is static. No build step is required.

1. Push these files to a GitHub repository.
2. Go to **Settings → Pages**.
3. Set source to **Deploy from a branch**.
4. Select your branch, usually `main`.
5. Select `/ (root)`.
6. Save.

GitHub Pages will serve `index.html`.

## Codex pet export notes

Codex package export builds:

- `spritesheet.webp`
- `1536×1872`
- `8×9` grid
- `192×208` frame cells
- `pet.json` pointing to `spritesheet.webp`

The first 9 loaded strips map to these rows:

1. idle
2. running-right
3. running-left
4. waving
5. jumping
6. failed
7. waiting
8. running / working
9. review

Open each strip with **Edit** if the source strip has fewer than 8 source frames.

## Privacy

Everything runs locally in your browser. Images are not uploaded anywhere.
