# HydroPrep WRE — PE Civil: Water Resources & Environmental CBT Suite (v3)

A 100% self-contained, offline-capable Progressive Web App (PWA) for the NCEES PE Civil: Water Resources & Environmental Computer-Based Test (CBT).

## What's New in v3
- **Natural Textbook Mathematical Typography**: All 276 practice problems, 96 NCEES Handbook v2.2 equations, and 12 section problem-setup guides use native HTML mathematical formatting (`<sub>`, `<sup>`, stacked fractions, square roots, and Greek symbols) with zero raw `^` or `_` characters. Works 100% offline and on GitHub Pages without external math CDN dependencies.
- **Section-Specific Formulas & Setup Guides in Topic Drills**: When drilling any of the 12 PE Civil WRE sections in Study Mode, the Section Formula Sheet & Problem-Solving Setup drawer automatically filters to that section's equations and setup methodology.
- **Full Handbook Access in CBT Exam Simulation**: During a timed CBT Exam Simulation, all 96 formulas across all 12 PE sections are searchable via the CBT Handbook modal.
- **Narrative Step-by-Step Engineering Solutions**: Every problem features a 4-stage engineering story walking through Problem Setup, NCEES Handbook v2.2 Strategy, Mathematical Walkthrough, and Field Sanity Check.

## Deploying to GitHub Pages
1. Upload all files in this ZIP archive (`index.html`, `manifest.json`, `service-worker.js`, `questions.json`, `formulas.json`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`) to the root of your GitHub repository.
2. Go to **Settings -> Pages**, select your branch (`main`) and root folder (`/`), and click **Save**.
3. If updating an existing deployment, hard-refresh (`Ctrl+Shift+R` or `Cmd+Shift+R`) so Service Worker `hydroprep-wre-v3` activates immediately.
