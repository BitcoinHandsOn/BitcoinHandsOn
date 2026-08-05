# BitcoinHandsOn.com

Static site for the book *Bitcoin Hands-On*. No build step, no JavaScript, no dependencies.

## Structure

- `index.html` — the whole page. Edit content directly.
- `css/style.css` — all styling. Colors and fonts are CSS variables at the top of the file.
- `assets/images/cover.jpg` — the book cover (add this — see below).
- `assets/images/card.jpg` — social sharing image (optional; referenced by og:image).
- `CNAME` — tells GitHub Pages to serve at bitcoinhandson.com.

## Before first deploy

(Images are already included.)
   site, and place it at `assets/images/cover.jpg`.
2. Optionally add `assets/images/card.jpg` (the social share image) the same way.

## Deploy to GitHub Pages

1. Create a repo (e.g. `bitcoinhandson`), push these files to `main`.
2. Repo Settings → Pages → Source: "Deploy from a branch" → `main` / root.
3. Settings → Pages → Custom domain: `bitcoinhandson.com` (the CNAME file handles this,
   but confirm it appears here). Check "Enforce HTTPS" once the cert is issued.

## DNS (at your registrar)

- Apex `bitcoinhandson.com` → A records:
  185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- `www` → CNAME → `<your-github-username>.github.io`

Propagation plus GitHub's certificate issuance can take up to an hour.

## Editing tips

- Retheme: change the hex values in `:root` at the top of `style.css`.
- Add an FAQ entry: copy any `<details>` block in the FAQ section.
- Add a resource: copy a `<dt>`/`<dd>` pair in the Resources section.
