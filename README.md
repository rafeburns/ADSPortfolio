# M.S. Applied Data Science Portfolio

ePortfolio site for **IST 782** (Syracuse University, M.S. in Applied Data Science).

## Structure

```
.
├── index.html          # Overview: learning outcomes, project summaries, mapping
├── projects.html       # Detailed project descriptions
├── video.html          # Embedded 1–2 minute video presentation
├── blog.html           # ~3,000 word reflection
├── assets/css/style.css
├── .nojekyll           # Tells GitHub Pages to serve files as-is (no Jekyll)
└── README.md
```

## How to fill it in

Search the site for `[YOUR NAME]`, `[PROJECT`, `[COURSE`, and `placeholder` — every spot that needs your content is bracketed. Suggested order:

1. Replace `[YOUR NAME]` everywhere (4 HTML files).
2. Fill in your three projects in [`projects.html`](projects.html).
3. Update the project cards and mapping table in [`index.html`](index.html).
4. Add your track in [`index.html`](index.html).
5. Embed your video in [`video.html`](video.html) (replace `REPLACE_WITH_VIDEO_ID`).
6. Write the blog post in [`blog.html`](blog.html).

## Local preview

Open `index.html` directly in a browser, or run a tiny local server:

```bash
# from this directory
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a new repo on GitHub. If you name it `<your-username>.github.io` it deploys to `https://<your-username>.github.io/`. Any other name deploys to `https://<your-username>.github.io/<repo-name>/`.
2. From this directory:

   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save.**
4. Wait ~1 minute. Your site will be live at the URL shown on the Pages settings page.

## Notes on the rubric

Mapping of rubric requirements (PDF page 2, section 2) to files:

| Requirement | Where it lives |
|---|---|
| a. Overview — outcomes, project summaries, mapping | [`index.html`](index.html) |
| b. Project descriptions (detailed) | [`projects.html`](projects.html) |
| c. Recorded video presentation (1–2 min) | [`video.html`](video.html) |
| d. Blog post (~3,000 words) | [`blog.html`](blog.html) |

The site is public by default. If you'd rather password-protect it, GitHub Pages doesn't support that natively — easiest route is to deploy on Netlify (free tier supports site-wide passwords), or keep the repo private and share screenshots/PDF for grading.
