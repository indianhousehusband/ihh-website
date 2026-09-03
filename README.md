# Indian House Husband — website

## What's in here
- `index.html` — homepage (hero + essay list)
- `about.html` — about page (with your full logo)
- `essays/` — 3 sample essay pages, pulled from your Medium posts
- `style.css` — shared styling, in navy/orange/sage to match your logo
- `logo.png` — your full logo, used on the about page
- `logo-header.png` — cropped version (no tagline strip), used in the site header
- `CNAME` — already set to `indianhousehusband.com`

## To go live on GitHub Pages
1. Create a new **public** repo on GitHub (e.g. `ihh-website`).
2. Upload every file in this folder as-is, keeping the `essays/` folder and the `CNAME` file intact.
3. In the repo, go to **Settings > Pages**, set Source to your main branch, root folder. Save.
4. At your domain registrar, add these A records pointing to GitHub:
   `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   (and a CNAME record for `www` pointing to `yourname.github.io`, if you want www to work).
5. Once DNS updates (can take a few hours), go back to Settings > Pages and check **Enforce HTTPS**.

## Adding more essays
Copy one of the files in `essays/`, swap in the new title, meta line, and paragraphs, then add a matching row to the essay list in `index.html`. Happy to do this in bulk whenever you're ready to bring over the rest of weeks 1-8.
