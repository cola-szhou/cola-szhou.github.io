# Shasha Zhou — Personal Homepage

A static homepage. No build step.

## Files
- `index.html` — the whole page
- `tweaks-panel.jsx` — in-page tweaks panel (optional; safe to delete if you don't want it)

## Run locally
Just double-click `index.html`, or:
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a new public repo on GitHub named **`<your-username>.github.io`**
   (e.g. `shashazhou.github.io`). This special name gets served at
   `https://<your-username>.github.io/` automatically.

2. Push these files to the `main` branch:
   ```bash
   cd site
   git init
   git add .
   git commit -m "initial homepage"
   git branch -M main
   git remote add origin git@github.com:<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```

3. In your repo on GitHub → **Settings → Pages** → make sure source is
   `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.

4. Wait ~1 minute and visit `https://<your-username>.github.io/`.

### Alternative: any repo name
If you'd rather use a normal repo (e.g. `homepage`), the site lives at
`https://<your-username>.github.io/homepage/`. Same steps; just enable Pages
in Settings → Pages.

## What to fill in before publishing
- Replace the portrait placeholder in `index.html`:
  search for `<div class="portrait">` and swap in `<img src="me.jpg" />`
  (put `me.jpg` next to `index.html`).
- Replace `#` social links in the hero (Scholar / GitHub / Twitter / ORCID).
- Replace `#` links on each publication (PDF / abs / bib / code).
- Update `News` items as new things happen.

## Editing tips
- Colors: change `--accent` near the top of the `<style>` block, or use the
  Tweaks panel during editing — it writes the new default back into the file.
- Fonts: swap the Google Fonts URL in `<head>`.
- Sections: each `<section>` is independent; cut/paste freely.
