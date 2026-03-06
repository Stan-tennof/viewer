# STEP Checker - Publish Ready (GitHub Pages)

Static web app for STEP preview and measurement.

## Files to keep in repo root
- `index.html`
- `vendor/three.min.js`
- `vendor/occt-import-js.js`
- `vendor/occt-import-js.wasm`
- `vendor/occt-import-js-worker.js`
- `.nojekyll`

## Deploy on GitHub Pages
1. Create a new GitHub repository.
2. Upload the project files (root + `vendor` folder).
3. In GitHub: `Settings` -> `Pages`.
4. Source: `Deploy from a branch`.
5. Branch: `main` and folder `/ (root)`.
6. Save.
7. Wait 1-2 minutes and open the Pages URL.

## Notes
- Browser-side only: users load STEP files from their own computer.
- No backend required.
- Keep vendor filenames exactly as referenced by `index.html`.
