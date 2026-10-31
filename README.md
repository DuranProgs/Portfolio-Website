# Deployment (Netlify, free, about 5 minutes)
1. Put your CV PDF in `files/` named `Johan-Carl-Duran-CV.pdf`.
2. Open index.html, sitemap.xml and robots.txt and replace `https://YOUR-SITE.netlify.app` with your real site URL.
3. Go to app.netlify.com > Add new site > Deploy manually, and drag this whole folder in. HTTPS is automatic.
4. `_redirects` makes clean URLs (/about, /projects/...) work. GitHub Pages does not support it.
5. Test: open the URL on your phone, click every menu item, open a project, search, view and download the CV, toggle theme, and submit sitemap.xml to Google Search Console.

# Updating content
Everything is in index.html: projects are the `P` array, experience the `E` array, education the `ED` array. Optional fields per project: url, gh, demo, y (year), role, st (status). Links appear only if you fill them in.

# Deploy on GitHub Pages
1. Create a GitHub repo named exactly `DuranProgs.github.io` (public). Your site will be https://duranprogs.github.io/
2. Upload everything inside this folder (index.html, 404.html, images/, files/, profile.jpg, robots.txt, sitemap.xml). Do not upload the folder itself.
3. Repo Settings > Pages > Source: Deploy from a branch > main / (root) > Save. Wait 1-2 minutes.
4. Your site URL (https://duranprogs.github.io) is already set in index.html, 404.html, sitemap.xml and robots.txt, so nothing to change.
`404.html` is a copy of index.html so direct links like /projects/flight-aviary still open the right page.
