# Lab Practical Timer

## Project
- Plain static site, no build step. The whole app is `index.html` (HTML, CSS and JS inline).
- Hosted on Vercel, which auto-deploys when `main` is pushed to GitHub
  (https://github.com/MrRankdizzle/lab-practical-timer). Never use the Vercel CLI.

## App behavior
- Themes: Classic, Histology, Fetal Pig. Each theme stores its own station count and
  times in localStorage under `"lpt-settings-v2"`.
- Phase labels must stay "Work Time" and "Rotate to Next Station".
- No emoji in the UI; use SVG icons.

## PWA cache
- If you change `sw.js`, `manifest.webmanifest`, or anything in `icons/`, bump the
  `CACHE` name in `sw.js` (e.g. `lab-practical-timer-v2` -> `-v3`) so installed copies update.

## Git workflow
- Commit with a clear message and push to `main` when I approve a change.
