# Tejo Girish Jonnavittula — Portfolio Site

Static site. No build step, no dependencies. Just `index.html` + `assets/`.

## Files
- `index.html` — the whole site (HTML/CSS/JS in one file)
- `assets/Tejo_Girish_Resume.pdf` — downloadable résumé, linked from the nav, hero, and contact section

## Deploy — Vercel (recommended, free, custom domain support)
1. Go to https://vercel.com and sign up / log in (GitHub login is easiest).
2. Click **Add New → Project**.
3. If your code isn't on GitHub yet, drag-and-drop the whole `tejo-portfolio` folder onto the "Deploy" screen instead (Vercel supports direct upload) — or push it to a new GitHub repo first (see below) and import that repo.
4. Framework preset: choose **Other** (it's a plain static site — no build command needed).
5. Click **Deploy**. In ~30 seconds you'll get a live URL like `tejo-girish.vercel.app`.
6. Optional: Project Settings → Domains → add your own domain.

## Deploy — Netlify (equally easy)
1. Go to https://app.netlify.com/drop
2. Drag the `tejo-portfolio` folder straight into the browser window.
3. Netlify deploys it instantly and gives you a live URL. Rename it under Site settings → Change site name.

## Deploy — GitHub Pages (free, ties to your GitHub profile)
1. Create a new GitHub repo, e.g. `tejo-portfolio`.
2. Push these files to it:
   ```bash
   cd tejo-portfolio
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/tejo-portfolio.git
   git push -u origin main
   ```
3. In the repo: Settings → Pages → Source → select `main` branch, `/ (root)` folder → Save.
4. Your site goes live at `https://<your-username>.github.io/tejo-portfolio/` within a minute or two.

## After deploying
- Add the live URL to your LinkedIn profile ("Featured" section or the headline URL field).
- Add it to your resume header next to your email.
- Test the résumé download link and the "Email me" button on mobile.

## Editing content later
Everything — copy, stats, links — lives in plain text inside `index.html`. Search for the section you want (`id="about"`, `id="experience"`, etc.) and edit directly; no rebuild needed, just re-upload/re-push the file.
