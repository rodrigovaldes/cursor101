# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **static HTML/CSS "Coming Soon" website** ("My Business"). It has no
package manager, no build step, no backend, no database, and no JavaScript. The pages are
`index.html`, `about.html`, `contact.html`, styled by `styles.css`.

### Running the site (dev)

Serve the repository root over HTTP (opening via `file://` works but is a weaker test because
the Content-Security-Policy and font loading behave differently):

```bash
python3 -m http.server 3000
# then open http://localhost:3000/
```

`npx serve` also works (documented in `README.md`), but it defaults to port 3000 as well and
downloads the `serve` package on first use; `python3 -m http.server` is preferred since Python
is already available with no network fetch.

### Lint / test / build

There are **no** lint, test, or build commands — nothing is defined and there is nothing to
compile. Deployment is the files as-is (see `README.md`).

### Non-obvious notes

- DM Sans and Manrope are self-hosted under `fonts/` (see `fonts/README.md`). No CDN or
  outbound network is required for typography.
- The `about.html` nav intentionally links back to `Home` and does not contain a `Contact Me`
  link — this is the site's design, not a bug.
- No environment variables or secrets are required.
