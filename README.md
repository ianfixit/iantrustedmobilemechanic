# Ian’s Mobile Mechanic — Static site

This repository contains a simple static site (index.html + styles). Follow the instructions below to run locally or publish to GitHub Pages.

## Quick local test (no server required)
- You can open `index.html` directly in your browser. For some browsers and local features a local server is recommended.

## Run with a simple static server
Option A — Python 3 (built-in):
```bash
# from repo root
python3 -m http.server 8000
# open http://localhost:8000 in your browser
```

Option B — Node (http-server):
```bash
npx http-server -c-1 8000
# open http://localhost:8000
```

Option C — Visual Studio Code
- Install the "Live Server" extension and click "Go Live".

## Files you should add/verify
- `styles.css` — present in repo root (this repo includes a ready-to-use file).
- `logo.png` — optional: place a logo file in the repo root or update the `img` src in `index.html`.
- Replace placeholder values:
  - Phone links in `index.html` are currently set to `+1 (858) 323-6041`. Update if needed.
  - Form action: replace `https://formspree.io/f/yourFormId` with your Formspree endpoint or another form backend.

## Publish on GitHub Pages (manual)
1. Commit and push your files to the `main` branch (or the branch you prefer).
2. On GitHub, go to the repository → Settings → Pages.
3. Under "Build and deployment", choose "Deploy from a branch".
4. Select the branch (`main`) and the folder (`/ (root)`), then Save.
5. GitHub will provide a Pages URL (it may take a minute to build).

Alternatively, you can use the `gh` CLI to publish or create a `gh-pages` branch.

## Troubleshooting
- If styles don't load: open DevTools → Console/Network and check for 404 on `styles.css` or `logo.png`. Ensure files are in repo root.
- If links not working on desktop (tel/sms): tel and sms links are mainly useful from a phone.
- Form not submitting: ensure you replaced the Formspree action with your endpoint and that CORS/allowed domain settings (Formspree) are configured.

## Want me to push these files?
If you'd like, I can add `styles.css` (and README) to the repo and create a commit/PR. Say:
- “Yes — push files” to proceed.
- Or ask for changes to the CSS before committing.
