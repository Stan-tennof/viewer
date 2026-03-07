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

## Project Structure
- `index.html`
- `vendor/three.min.js`
- `vendor/occt-import-js.js`
- `vendor/occt-import-js.wasm`
- `vendor/occt-import-js-worker.js`

## Run Locally
From project root:

```powershell
py -m http.server 8000 --bind 127.0.0.1
```

Open:

`http://127.0.0.1:8000/index.html`

If you changed files, hard refresh with `Ctrl+F5`.

## Controls
- Left drag: rotate
- Right drag: pan
- Mouse wheel: zoom
- Left click: select part / pick A-B points
- Right click (no drag) on part: hide confirmation

## GitHub Pages Deploy
1. Push this repository to GitHub.
2. Go to `Settings` -> `Pages`.
3. Source: `Deploy from a branch`.
4. Branch: `main`, folder: `/ (root)`.
5. Save and wait 1-2 minutes.

Your site URL will be:

`https://<username>.github.io/<repo>/`

## Notes
- Fully client-side: no server backend.
- STEP files are processed in browser memory only.
- Keep `vendor` filenames and paths unchanged.
