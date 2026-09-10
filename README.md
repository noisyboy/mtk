# Materials Science Toolkit

A modular, client-side web application designed to assist with calculations for materials science, solid-state physics, and perovskite research. The toolkit runs entirely in the browser and is optimized for static hosting environments like GitHub Pages.

## Included Tools

* **Sol-Gel Precursor Calculator:** Calculates the required masses for sol-gel synthesis of complex perovskites (ABX3). It supports fractional stoichiometry, mixed A/B/X sites, purity adjustments, and custom chelating agent ratios (e.g., Citric Acid, EDTA). Users can utilize the built-in database of common nitrates, carbonates, and acetates, or input custom molar masses dynamically.
* **Goldschmidt Tolerance Factor Calculator:** Predicts the structural stability of perovskite solid solutions. It calculates the tolerance factor (t) based on fractional occupancies using a built-in database of Shannon effective ionic radii mapped to their standard coordination numbers (A-site = 12, B-site = 6, X-site = 6). It includes support for high-spin/low-spin states and custom ionic radii inputs.

## Architecture

This project is built using vanilla HTML, CSS, and JavaScript. It uses a scalable, iframe-based hash routing architecture that isolates the CSS and JavaScript of each calculator to prevent namespace collisions.

Adding a new calculator requires zero structural changes to the UI. Developers only need to upload the standalone HTML file and append a single line to the configuration object in `index.html`:

```javascript
const tools = {
    'sol-gel': { title: 'Sol-Gel Calculator', file: 'sol-gel.html' },
    'tolerance': { title: 'Tolerance Factor', file: 'tolerance.html' },
    // Add new tools here
};

```

## Deployment

The application requires no backend, database, or build steps (like Node/NPM). It can be deployed directly by serving the repository directory via GitHub Pages, Apache, Nginx, or any standard static file server.
or use it online hosted [here](https://noisyboy.qzz.io/mtk/)
