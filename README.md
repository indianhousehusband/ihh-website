# Indian House Husband — website

## What's in here
- `index.html` — homepage (hero + essay list)
- `about.html` — about page (with your full banner)
- `essays/` — 3 sample essay pages, pulled from your Medium posts
- `style.css` — shared styling, in navy/orange/sage to match your logo, fully responsive
- `logo.png` — square icon version, used as the favicon
- `logo-header.png` — cropped version (no tagline strip), used in the site header/nav
- `banner.png` — full logo with tagline, used full-width on the about page and as the social preview image
- `robots.txt` and `sitemap.xml` — for search engine indexing
- `CNAME` — already set to `indianhousehusband.com`

## To go live on GitHub Pages
1. Create a new **public** repo on GitHub (e.g. `ihh-website`).
2. Upload every file in this folder as-is, keeping the `essays/` folder and the `CNAME` file intact.
3. In the repo, go to **Settings > Pages**, set Source to your main branch, root folder. Save.
4. At your domain registrar, add these A records pointing to GitHub:
   `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   (and a CNAME record for `www` pointing to `yourname.github.io`, if you want www to work).
5. Once DNS updates (can take a few hours), go back to Settings > Pages and check **Enforce HTTPS**.

## Getting indexed on Google
The site now has the on-page basics in place: unique titles/descriptions per page, canonical links, Open Graph and Twitter card tags for social previews, structured data (schema.org) on the homepage and each essay, plus `robots.txt` and `sitemap.xml`. To actually get crawled faster instead of waiting for Google to stumble onto it:
1. Go to [Google Search Console](https://search.google.com/search-console) and add `indianhousehusband.com` as a property (choose the "Domain" property type, which verifies via a DNS TXT record at your registrar).
2. Once verified, go to **Sitemaps** in the left menu and submit `https://indianhousehusband.com/sitemap.xml`.
3. Use **URL Inspection** on your homepage and click "Request Indexing" to speed things up further.
4. Every time you add a new essay page, add its URL to `sitemap.xml` and resubmit (Search Console will pick up the update automatically once the sitemap file changes, but a manual resubmit doesn't hurt).

## Adding more essays
Copy one of the files in `essays/`, swap in the new title, meta line, and paragraphs, then add a matching row to the essay list in `index.html`. Also add the new page's URL to `sitemap.xml` so it gets indexed. Happy to do this in bulk whenever you're ready to bring over the rest of weeks 1-8.
