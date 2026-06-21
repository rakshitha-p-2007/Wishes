# Father's Day Special — Static Webpage

This is a small, static webpage located in the `docs/` folder. It is ready to be published as a static site (GitHub Pages) or deployed to Vercel.

Quick checklist before creating a new repository and deploying:

- Add your image and audio assets into the `docs/` folder (e.g. `bf-photo.png`, `first-date.jpeg`, `audio.mp3.ogg`). If you don't provide images, the site will automatically use placeholder images.
- Install Node.js if you plan to use the Vercel CLI or other Node tooling.

How to initialize a new Git repository and push (example):

```powershell
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Deploy options:

- GitHub Pages (uses the `docs/` folder):
  1. Push to GitHub.
  2. In the repository Settings → Pages, set the source to branch `main` and folder `/docs`.
  3. Save — your site will be available at `https://<your-username>.github.io/<repo-name>/`.

- Vercel (recommended for simple deploys):
  - Option A: Import the repo at https://vercel.com (one-click deploy)
  - Option B (CLI): install Node.js, then run:
```powershell
npm i -g vercel
vercel login
vercel --prod
```

Notes:
- If you want to keep everything purely static with no build step, GitHub Pages or Vercel will serve the files directly from `docs/`.
- The page includes automatic fallbacks for missing images (remote placeholders) and a hint for audio — add `audio.mp3.ogg` to `docs/` to enable the surprise message.

If you want, I can:
- create a minimal `index.html` variant at the repo root, or
- set up a GitHub Actions workflow to automatically deploy to GitHub Pages.
