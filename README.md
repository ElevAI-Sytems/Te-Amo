# Te Amo Padel

Marketing website for **Te Amo Padel** — community-first padel at The Hayes, Alvechurch, Birmingham. Three outdoor courts, café & bar, and coaching. Open 6am–10pm daily.

## Overview

A single-page static site built with plain HTML, CSS, and vanilla JavaScript — no build step or dependencies. Everything is contained in `index.html`, which loads images, video, and Google Fonts.

```
.
├── index.html        # the entire site
└── assets/           # images and video referenced by index.html
```

## Run locally

Because the page loads a video and images, open it through a local web server rather than the `file://` protocol:

```bash
# Python 3
python -m http.server 8000
# then visit http://localhost:8000
```

Or simply open `index.html` directly in a browser — most things work, though some browsers restrict autoplay/video over `file://`.

## Deploy

Any static host works (GitHub Pages, Netlify, Vercel, Cloudflare Pages). The entry point is `index.html` at the repository root.

For **GitHub Pages**: enable Pages in repository settings and serve from the default branch root. Add an empty `.nojekyll` file if you later introduce folders that begin with an underscore.

## Booking

Court bookings are handled through [Playtomic](https://playtomic.io/).
