# HydroPrep WRE — PWA Deployment Guide

## Files Included in this Package
- `index.html`: Complete single-file application with embedded question bank, NCEES Reference Handbook v2.2 formulas, CBT exam simulator, adaptive drills, and Service Worker registration.
- `manifest.json`: Web App Manifest defining the PWA metadata, standalone display mode, theme colors, and icons.
- `service-worker.js`: Offline caching engine with immediate activation (`skipWaiting` + `clients.claim`) and navigation fallback.
- `icon-192.png`: 192x192 PNG app icon (Android Home screen & splash).
- `icon-512.png`: 512x512 PNG app icon (Android high-res launcher).
- `apple-touch-icon.png`: 180x180 PNG icon for iOS Safari.
- `questions.json`: Raw JSON database of all 35 verified PE Civil WRE exam problems and step-by-step solutions.

---

## How to Update Your GitHub Repository

1. **Extract all files** from `pe_wre_pwa.zip`.
2. **Copy and replace** all extracted files into the root folder of your GitHub repository.
3. **Commit & Push** your changes to GitHub:
   ```bash
   git add .
   git commit -m "Enable PWA installation: add service worker, manifest, icons, and install prompt"
   git push origin main
   ```
   *(Or drag-and-drop the files directly through the GitHub.com web interface and click "Commit changes".)*
4. Ensure GitHub Pages is enabled in **Settings -> Pages** (pointing to your `main` branch, `/ (root)` folder).

---

## How to Install / Download to Your Phone

### On Android (Google Chrome, Samsung Internet, Microsoft Edge):
1. Open your GitHub Pages URL on your phone: `https://<your-username>.github.io/<repo-name>/`.
2. You will now see a green **"Install App"** button in the header and an **"Install App on Phone"** button in the dashboard hero banner.
3. Tap either button to trigger the native Android installation prompt!
4. Alternatively, tap the **three dots (⋮)** in the top-right corner of Chrome and select **"Install app"** (or **"Add to Home screen"**).
5. Tap **"Install"**. The app will now be saved on your home screen like any native app and will launch in full screen with offline support.

### On iPhone / iPad (Apple Safari):
1. Open your GitHub Pages URL in Safari.
2. Tap the **Share** button (square with arrow pointing up) at the bottom toolbar.
3. Scroll down and tap **"Add to Home Screen" (+)**.
4. Tap **"Add"** in the top-right corner.
