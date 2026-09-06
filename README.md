# The Parkline Classic — Website

A 9-page static site for The Parkline Classic (hotel & restaurant, Agartala): `index.html`, `about.html`, `rooms.html`, `dining.html`, `gallery.html`, `contact.html`, `404.html`, plus `robots.txt` and `sitemap.xml`. All pages share `styles.css` and `main.js`, and the seal logo `parkline-seal.png` sits at the top level alongside them (no `images/` subfolder).

## Before this goes live

A few things are placeholder on purpose and should be swapped before the site is public:

- **Photos** — the rooms, food and property shots are stock photography (Unsplash), used to show the layout while real photos aren't available yet. Swap them for actual photos of the hotel and kitchen before launch; the `img` and `data-full` attributes in `index.html` and `gallery.html` are the ones to update, and the corresponding `alt` text should be updated to match.
- **Reservation form** — the form on `contact.html` currently just shows a front-end confirmation message (see `main.js`); it isn't wired up to anything yet. Before launch, connect it to email, WhatsApp, or whatever booking system the hotel wants to use.
- **Domain** — `robots.txt`, `sitemap.xml`, and the canonical/Open Graph tags in each page's `<head>` currently point at a placeholder domain (`https://www.theparklineclassic.in`). Once the real domain is confirmed, find-and-replace that placeholder across all files.

## How to put this on GitHub

1. **Unzip this download first** — you should end up with a folder containing the 7 `.html` files, `styles.css`, `main.js`, `parkline-seal.png`, `robots.txt`, and `sitemap.xml`, all at the same level. Do not upload the `.zip` itself to GitHub — GitHub does not open zip files.

2. Go to **github.com** → click **New repository** → name it (e.g. `parkline-classic-website`) → **Create repository** (leave it empty, no README needed).

3. On the new repo page, click **Add file → Upload files**.

4. Open the unzipped folder on your computer, select **all the files together**, and drag them all into the GitHub upload box in one go. Scroll down and click **Commit changes**.

5. Check the file list on GitHub afterwards — `index.html`, `styles.css`, `main.js`, and `parkline-seal.png` should all be sitting at the **top level** of the repo (not inside an extra subfolder). If GitHub shows a folder like `parkline-classic-website/index.html` instead of just `index.html`, open that folder and move the files up, or re-upload selecting the *contents* of the folder rather than the folder itself.

6. To get a live, shareable link: go to **Settings → Pages** in the repo → under "Source" choose **Deploy from a branch**, branch `main`, folder `/ (root)` → **Save**. Wait about a minute, then your site is live at:

   `https://<your-username>.github.io/parkline-classic-website/`

That live link is what to send the hotel for review — it shows the fully styled site, not just code.
