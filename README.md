# Marieswaran S — Portfolio

A single-file portfolio site styled like a redacted penetration-test report — terminal-style hero, engagement timeline, and a findings table for disclosed research.

Live in one file: `index.html` (CSS and JS are inline, no build step, no dependencies to install).

## Put this on GitHub Pages (free hosting)

1. Create a new repository on GitHub — name it `portfolio` (or anything you like). If you name it `<your-username>.github.io`, it'll be live at the root of that URL instead of a subpath.
2. Upload `index.html` to the repository (drag-and-drop on the GitHub web UI works, or use git):
   ```bash
   git init
   git add index.html
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute, then your site is live at:
   `https://<your-username>.github.io/<repo-name>/`
   (or `https://<your-username>.github.io/` if you named the repo `<your-username>.github.io`)

## Editing content later

Everything is in `index.html` — search for the section you want to change:
- `#summary` — the executive-summary text block
- `#experience` — each `.engagement` card is one job
- `#findings` — the disclosures table (`<table class="findings">`)
- `#skills` — chip tags grouped by category
- `#certs` — the certification grid
- `#contact` — email, phone, LinkedIn, portfolio link

No build tools, no npm install — just edit the HTML and refresh.
