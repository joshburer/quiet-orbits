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
- **Palettes.** 15 hand-tuned palettes from 2 to 16 colours. The scene is rendered
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
| Click a world | Visit it (click empty sky to return) |
| Space or R | Random system |
| Left / Right | Previous / next world |
| Up / Down or P | Palette |
| D, X, M | Dither pattern, pixel size, journey mode |
| O, C, L | Orbit lines, constellation lines, name captions |
| F, Esc | Fullscreen, back to the whole system |

The control strip hides after a few seconds without input.
