# States of Matter – A 3D Journey into the World of Particles
Interactive 3D science lab (PWA) for Classes 5–6. Developed by Mateen Yousuf, Teacher.

## Files
`index.html` (all UI, CSS, JS, content) · `manifest.json` · `service-worker.js` · `offline.html` · `three.min.js` (Three.js r149, local – no CDN) · `icons/`
No backend, login or API key.

## Run it
Service workers (offline mode and installing) need **HTTPS or http://localhost**. Opening index.html directly (file://) shows the app, but offline saving and install are unavailable.
```
cd matter_pwa
python3 -m http.server 8080      # then open http://localhost:8080
```
## Deploy
Upload the whole folder to any HTTPS static host (GitHub Pages, Netlify, school server). Keep files together in one folder.

## Install on Android
Open the site in Chrome → tap **Install App** (top bar) or menu ⋮ → *Install app / Add to Home screen*. iPhone/iPad: Safari → Share → *Add to Home Screen*.

## Check offline works
1. Open the site once while online. Help → ℹ should say “✔ Saved for offline use”.
2. Turn on airplane mode (or DevTools → Network → Offline), reload: the app still opens; the top bar shows “Offline – using saved files”.

## Updating
Change `VERSION` in `service-worker.js` after editing any file. Users see “A new version is ready – Refresh”.

## Contents
Particle Laboratory (3 chambers + temperature & motion), Heating/Melting, Freezing, Evaporation vs Boiling, Condensation, Sublimation & Deposition, Compare States, Real-Life Explorer (10 items), interactive Changes-of-State diagram (🔄), Activities A–C, Quiz (15 of 25 questions), Glossary, Help. Presentation mode, low-graphics mode, keyboard support.

## Notes on accuracy
All models are simplified: particles are enlarged, speeds exaggerated, heating curves not to scale. Phase-change temperatures depend on substance and pressure.
