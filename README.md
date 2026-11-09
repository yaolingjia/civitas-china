# Civitas China — marketing site

Static single-page site for **Civitas China** (California-registered company · Beijing delivery studio).

English-first copy for California architecture firm Principals / Production leaders. No build step.

## Contents

| Path | Purpose |
|------|---------|
| `index.html` | Full landing page |
| `styles.css` | Studio grayscale + lavender accent |
| `script.js` | Mobile nav toggle |
| `assets/logo.png` | Full logo |
| `assets/logo-mark-160.png` | Header / favicon source mark |
| `assets/favicon.png` | Favicon |
| `assets/cases/` | Selected China project thumbnails (credential illustration) |

## Local preview

```bash
cd civitas-china-site
python3 -m http.server 8080
# open http://localhost:8080
```

Or open `index.html` directly in a browser.

## Deploy free on GitHub Pages (you own the repo)

This is the recommended free, permanent hosting path. **You** create and own the GitHub repository; Pages stays free for public repos.

### 1. Create a repo under your GitHub account

1. Sign in at [github.com](https://github.com) (create an account if needed).
2. **New repository** → name e.g. `civitas-china` (or `civitas-china.github.io` for a user/org site).
3. Keep it **Public** (required for free GitHub Pages on personal accounts without paid extras).
4. Do **not** initialize with a README if you will push this folder as-is.

### 2. Push this site

From a machine with Git installed:

```bash
cd civitas-china-site
git init
git add .
git commit -m "Initial Civitas China marketing site"
git branch -M main
git remote add origin https://github.com/<YOUR_USERNAME>/<YOUR_REPO>.git
git push -u origin main
```

Replace `<YOUR_USERNAME>` and `<YOUR_REPO>` with your account and repo name.

### 3. Turn on GitHub Pages

1. Repo → **Settings** → **Pages**
2. **Source**: Deploy from a branch
3. **Branch**: `main` / folder `/ (root)` → Save
4. Wait 1–2 minutes. Your site URL will be:

`https://<YOUR_USERNAME>.github.io/<YOUR_REPO>/`

If the repo is named `<YOUR_USERNAME>.github.io`, the URL is:

`https://<YOUR_USERNAME>.github.io/`

### 4. Optional custom domain (still free DNS you control)

1. Buy or use a domain you own (e.g. Namecheap, Cloudflare, Google Domains).
2. In GitHub Pages settings, add the custom domain (e.g. `civitaschina.com`).
3. At your DNS provider, add the records GitHub shows (usually `A` / `CNAME`).
4. Enable **Enforce HTTPS** once DNS propagates.

Ownership: the GitHub repo, Pages site, and any custom domain stay under **your** accounts.

### Alternatives (also free / free tier)

- **Cloudflare Pages** — connect the same GitHub repo; free SSL + CDN.
- **Netlify** — drag-and-drop this folder or connect Git; free tier.
- **Vercel** — same pattern for static sites.

GitHub Pages is enough for a permanent brochure site with zero cost.

## Brand / legal notes for editors

- Civitas China is an **independent** California-registered company with a Beijing delivery studio.
- Frame credentials as **China–U.S. / U.S.–China collaboration projects** — do not name other firms.
- Contact email on the site: `yaolingjia@126.com`
- Do not invent phone numbers or street addresses.
- Services exclude Construction Documents (CD).

## Updating the site

Edit `index.html` / `styles.css`, commit, and `git push`. Pages rebuilds automatically.
