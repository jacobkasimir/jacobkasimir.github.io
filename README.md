# Portfolio – Jacob Tietz

Static site (HTML, CSS, a little JavaScript). No build step, no frameworks, no tracking.

## Files
- `index.html` (English) and `de.html` (German) – single page: Intro, Projects, Experience, Education, Skills, CV; contact icons in the footer
- `style.css`, `script.js`
- `404.html` – custom error page
- `assets/` – photo, logo/favicons, project images, CV PDFs (EN + DE, without phone number); PDFs open in a new browser tab
- `_unpublished/` – seminar papers, not deployed (ignored by git)
- `.nojekyll` – tells GitHub Pages to serve files as they are

## Preview locally
```bash
cd ~/Claude/Personal/portfolio
python3 -m http.server 8000
```
Open http://localhost:8000.

## Deploy to GitHub Pages
1. Create a **public** repo named `jacobkasimir.github.io` on GitHub.
2. In this folder:
   ```bash
   git init -b main
   git add .
   git commit -m "Initial portfolio"
   git remote add origin git@github.com:jacobkasimir/jacobkasimir.github.io.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`, Save.
4. After a minute the site is live at `https://jacobkasimir.github.io/`.

Before pushing, search for `TODO` and fill in or remove every placeholder (see `TODO.md`).
