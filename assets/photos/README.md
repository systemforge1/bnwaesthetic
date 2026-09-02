# Marvin's hero photo

This is the **only** image the site uses. Everything else is drawn in CSS.

**Installed:** `marvin.webp` — a transparent cut-out, ~90 KB, wired into the hero.
The original upload is kept here as `image.png` in case it needs re-exporting.

## Replacing it

Export a new cut-out and save it as `marvin.webp` (or `marvin.png` — then update
the `<img src>` in `index.html`). What works best:

| | |
|---|---|
| **Format** | Transparent background (cut-out, no backdrop) — WebP or PNG |
| **Crop** | Head + shoulders, or head to mid-torso |
| **Headroom** | Crop tight — top of his head near the top edge, little empty space above |
| **Framing** | Subject centred, looking toward camera |
| **Size** | ~1200 px tall, portrait-ish (it renders up to 900 px tall) |
| **Bottom edge** | Let the shoulders run to the bottom of the canvas — the page fades them out with a gradient mask |
| **Weight** | Aim under ~150 KB so the page stays light |

The hero layers this image **on top of the giant outlined name**, so his head
crosses through the letterforms. That effect only works with a cut-out — a photo
with its original background will just cover the type.

## No transparent version?

- [remove.bg](https://remove.bg)
- Photoshop → Select Subject → Layer Mask
- iPhone: long-press the subject in Photos → Copy

## If the file is missing

The hero shows a labelled upload slot instead of breaking, and nothing else on
the page depends on this file.
