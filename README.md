# Quiet Orbits

A browser screensaver that drifts through procedurally generated solar systems,
drawn low-res in a limited palette with ordered dithering.

**Play it:** https://joshburer.github.io/quiet-orbits/

Or open `index.html` in a browser. It is one self-contained file with no build step;
the only external request is the UI font from Google Fonts. GitHub Pages serves it
straight from the root of `main`.

## What it does

- **Seeds.** Any text is a seed, and the same seed always makes the same system.
  Simple seeds (letters, digits, hyphens) are written to the URL hash for sharing.
- **Worlds.** Each system has a star, 3–8 worlds of eight types (living, ocean,
  desert, ice, molten, barren, shrouded, gas giant), moons, the occasional
  asteroid belt, and rarely rings — banded or chunky debris.
- **Palettes.** 67 palettes from 2 to 32 colours, picked from a dropdown grouped by
  size: 34 made for this project (including three light "paper" ones) and 33
  community palettes of 16 to 32 colours from [Lospec](https://lospec.com/palette-list). The scene is rendered
  in linear colour, then every pixel is mapped to the best pair of palette
  colours and a mix ratio.
- **Dithering.** Bayer 2/4/8, halftone, scanline, hatch, grain or none, with an
  amount slider and three pixel sizes.
- **Journey.** *Wander* tours a few worlds then drifts to a new system, *Tour*
  stays in the current system, *Still* holds the view.

## Controls

| Input | Action |
| --- | --- |
| Drag / scroll | Turn the camera / zoom |
| Click a world | Jump to it (click empty sky to return) |
| Space or R | Random system |
| Left / Right | Previous / next world |
| Up / Down or P | Palette |
| D, X, M | Dither pattern, pixel size, journey mode |
| O, C, L | Orbit lines, constellation lines, name captions |
| F, Esc | Fullscreen, back to the whole system |
| H | Hide or show the control strip |

The control strip hides after a few seconds without input. **Hide** (or H) keeps it
away until you press **Menu** or H again. Worlds you pick by hand arrive in well under
a second; the slow camera moves are kept for the tour.

## Palette credits

The 16 to 32 colour community palettes come from the
[Lospec palette list](https://lospec.com/palette-list), with colours exactly as
published there. Authors are given as Lospec lists them.

| Palette | Colours | Author |
| --- | --- | --- |
| Sweetie 16 | 16 | not listed |
| PICO-8 | 16 | not listed |
| DawnBringer 16 | 16 | not listed |
| Endesga 16 | 16 | ENDESGA |
| Steam Lords | 16 | Slynyrd |
| NA16 | 16 | Nauris |
| Arne 16 | 16 | not listed |
| Island Joy 16 | 16 | Kerrie Lake |
| Bubblegum 16 | 16 | PineappleOnPizza |
| AAP-16 | 16 | Adigun A. Polack |
| Europa 16 | 16 | Star |
| Night 16 | 16 | not listed |
| Vanilla Milkshake | 16 | Space Sandwich |
| Galaxy Flame | 16 | Rhoq |
| Commodore 64 | 16 | not listed |
| Urbex 16 | 16 | Rustocrat |
| Taffy 16 | 16 | PineappleOnPizza |
| SLSO-CLR17 | 17 | Luis Miguel Maldonado |
| Autumn Glow | 20 | Sonnenstein |
| Punolit | 21 | Punoli |
| Fantasy 24 | 24 | not listed |
| Vinik24 | 24 | Vinik |
| CC-29 | 29 | Alpha6 |
| DawnBringer 32 | 32 | not listed |
| Endesga 32 | 32 | ENDESGA |
| Zughy 32 | 32 | not listed |
| Resurrect 32 | 32 | Kerrie Lake |
| Mulfok32 | 32 | mulfok |
| Nanner 32 | 32 | Afterimage |
| Jehkoba32 | 32 | Jehkoba |
| Hept32 | 32 | ENDESGA |
| Pineapple 32 | 32 | PineappleOnPizza |
| Sheltzy32 | 32 | NatTorpedia |
