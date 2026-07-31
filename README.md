# My Business — Coming Soon

A simple static "coming soon" website for My Business.

## Tech

- Plain HTML5 + CSS3
- Google Fonts (DM Sans, Manrope) via CDN
- No build step, no dependencies, no JavaScript

## Project structure

```
index.html    Main landing page (links to about and contact)
about.html    About page
contact.html  Contact page
styles.css    Shared styles
```

## Running locally

Open `index.html` directly in a browser, or serve the folder:

```bash
npx serve
# or
python3 -m http.server
```

## Deployment

Works as-is on any static host — GitHub Pages, Netlify, or Vercel. Just point it at this directory; no configuration needed.
