# STEP Viewer (Web)

Lightweight web STEP viewer focused on fast visual validation and simple measurements.

## Features
- Load `.step` / `.stp` directly in browser
- 3D navigation: rotate, pan, zoom
- Part selection + `Part Measurements`
- `Global Measurements` for full model bounds
- `2 points` measurement mode (A/B) with:
  - vertex snap
  - axis constraint (`Free`, `X`, `Y`, `Z`)
- Visibility tools:
  - `Isolate`
  - `Hide`
  - `Show all`
  - right click on a part -> hide confirmation
- Units: `mm` / `inch`

## Notes
- Fully client-side: no server backend.
- STEP files are processed in browser memory only.
- Keep `vendor` filenames and paths unchanged.
