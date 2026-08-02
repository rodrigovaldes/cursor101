# My Business — Coming Soon

A simple static "coming soon" website for My Business.

## Tech

- Plain HTML5 + CSS3
- Self-hosted fonts (DM Sans, Manrope; SIL Open Font License)
- No build step, no dependencies, no JavaScript

## Project structure

```
index.html    Main landing page (links to about and contact)
about.html    About page
contact.html  Contact page
styles.css    Shared styles
fonts/        Self-hosted woff2 font files
```

## Running locally

Open `index.html` directly in a browser, or serve the folder:

```bash
npx serve
# or
python3 -m http.server
```

## Deployment

Works as-is on any static host — GitHub Pages, Netlify, or Vercel. Just point it at this directory; no build step needed.

Security headers beyond the HTML CSP meta tags:
- Netlify reads `_headers` (`nosniff`, `X-Frame-Options`, `Permissions-Policy`, COOP/CORP, HSTS, CSP including `frame-ancestors`)
- Vercel reads `vercel.json` for the same header set
- GitHub Pages does not support custom response headers; the page-level CSP + referrer meta tags still apply
