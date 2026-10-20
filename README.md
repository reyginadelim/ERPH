# PH Emergency — Philippine Hospital Directory

A responsive one-page dashboard for tracking **documented annual emergency department visit counts** at selected major Philippine hospitals.

## Quick start
- Open `index.html` in a browser. No installation, dependencies, or build steps.
- Search by name/location, filter regions, and sort by available case counts.
- Select **Edit cases** to enter a count, reporting year, and source. Entries are kept in that browser's `localStorage`.
- Select **Export CSV** to save your data. Use this export as your backup, especially before clearing your browser storage.

## Important data limitations
This is **not a verified ranking of the highest-ER-volume hospitals**. Most hospital-level emergency department volumes are not published in a standardized, comparable format. The dashboard intentionally starts with **unreported** counts, never invented values. User-entered counts are not independently verified. A sum of entered cases is **not** a national estimate.

Hospital photos are requested from Wikipedia's public thumbnail API at runtime and require internet access. Where a relevant photo is unavailable, the bundled local SVG illustration is shown. Map links open Google Maps searches for the hospital/address. Independently check locations and reports before operational decisions.

## File structure
```
index.html
css/style.css
js/app.js
assets/hospital-placeholder.svg
README.md
```

## Publish to GitHub Pages
1. Create a GitHub repository and upload the **contents** of this folder (keep `index.html` in the repository root).
2. Go to **Settings → Pages → Deploy from a branch**.
3. Choose **main** and **/(root)**, then save.
4. Use the GitHub Pages URL displayed by GitHub once deployed.

## Tech
Vanilla HTML/CSS/JavaScript. Raleway is loaded via Google Fonts when online, with Arial fallback. No frameworks and no build tools.
