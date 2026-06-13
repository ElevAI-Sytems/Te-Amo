# Te Amo Padel

Marketing website for **Te Amo Padel** — community-first padel at The Hayes, Alvechurch, Birmingham. Three outdoor courts, café & bar, and coaching, open 6am–10pm daily.

## Overview

A single-page static website built as one self-contained `index.html` (HTML, CSS, and JavaScript inline). All images and videos live in `assets/`. No build step, no dependencies, no framework — just open it in a browser.

## Project structure

```
.
├── index.html        # The entire site (markup, styles, scripts)
└── assets/           # Images and videos referenced by index.html
    ├── hero-aerial.jpg
    ├── hero-video.mp4
    ├── location-aerial.mp4
    ├── section-bg.mp4
    ├── logo.jpg
    └── ...
```

## Running locally

Because the page loads video files, open it through a local web server rather than double-clicking the file (some browsers block local video over the `file://` protocol):

```bash
# Python 3
python3 -m http.server 8000
```

Then visit <http://localhost:8000> in your browser.

## Deploying

This is a static site, so it can be hosted anywhere that serves files:

- **GitHub Pages** — Settings → Pages → deploy from the `main` branch (root).
- **Netlify / Vercel / Cloudflare Pages** — drag-and-drop the folder or connect this repo; no build command needed.

## Fonts

Fonts (Bricolage Grotesque, Grand Hotel, Hanken Grotesk) are loaded from Google Fonts at runtime, so an internet connection is needed for the intended typography.

## Booking

Court bookings are handled via Playtomic (linked from the site).
