[README.md](https://github.com/user-attachments/files/30225424/README.md)
# Hritika Mithani — Portfolio Website

A responsive, editorial portfolio site. Static HTML/CSS/JS with self-hosted fonts and
optimised images — no build step, no dependencies. Loads fast and works offline.

## Contents
```
index.html            The whole site (HTML + CSS + JS in one file)
assets/img/           Project images + portrait (web-optimised)
assets/fonts/         Self-hosted Fraunces + Archivo (woff2)
_headers              Long-cache rules for Netlify
```

## Deploy (Netlify — easiest)
1. Go to app.netlify.com → "Add new site" → "Deploy manually".
2. Drag this whole folder onto the drop zone.
3. Done — you'll get a live URL. Add a custom domain later under Site settings → Domain.

## Deploy (GitHub Pages)
1. Create a repo and upload these files to the root.
2. Settings → Pages → Branch: `main` / root → Save.
3. Your site publishes at `https://<user>.github.io/<repo>/`.

## Two things to set before you publish
1. **LinkedIn link.** In `index.html`, near the very bottom, find:
   `document.getElementById('liLink').setAttribute('href','#');`
   Replace `#` with your LinkedIn URL, e.g. `https://www.linkedin.com/in/hritika-mithani`.
2. **Download CV.** Add your CV as `assets/Hritika-Mithani-CV.pdf`
   (the "Download CV" button already points there). Or change the path in the same
   script block: `document.getElementById('cvLink').setAttribute('href', ...)`.

## Editing content
All project text and images live in the `PROJECTS` array inside `index.html`
(search for `const PROJECTS`). Titles, locations, areas and descriptions are plain
text — edit them there. To swap an image, replace the matching file in `assets/img/`.

## Notes
- Fonts are bundled, so nothing loads from Google — reliable and private.
- Fully responsive (desktop → mobile), keyboard accessible, respects reduced-motion.
