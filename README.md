# halaa-pages

Public GitHub Pages site for the Halaan 1490 (حالا) store-listing web pages.

The app's source repo, [`ababeel-soft/halaa`](https://github.com/ababeel-soft/halaa), stays **private**. This repo contains only public HTML pages — no app code, signing keys, or credentials.

## Pages

| File | Default GitHub Pages URL | Current production URL |
|---|---|---|
| `index.html` | https://ababeel-soft.github.io/halaa-pages/ | — |
| `privacy.html` | https://ababeel-soft.github.io/halaa-pages/privacy.html | https://privacy.haalan.ly/ |
| `support.html` | https://ababeel-soft.github.io/halaa-pages/support.html | https://support.haalan.ly/ |
| `delete-account.html` | https://ababeel-soft.github.io/halaa-pages/delete-account.html | https://delete-account.haalan.ly/ |
| `marketing.html` | https://ababeel-soft.github.io/halaa-pages/marketing.html | https://marketing.haalan.ly/ |

## Source of truth

The files here are copied from `store-listing/` in the private `halaa` repo. Keep them in sync with that repo; do not make policy-content changes only here.

## Custom domains (optional)

GitHub Pages allows one custom domain per project site. To keep the existing `*.haalan.ly` URLs while serving them from this repo:

1. In **Settings → Pages → Custom domain**, add the desired domain (for example `privacy.haalan.ly`) and save. This commits a `CNAME` file at the repo root.
2. In DNS, create a `CNAME` record for that subdomain pointing to `ababeel-soft.github.io` (do **not** include the repo name).
3. Enable **Enforce HTTPS** once GitHub has issued the certificate.
4. Repeat from a separate Pages repo for each additional hostname, or use one docs hostname with path-based URLs.

Until DNS is changed, the production URLs above continue to be served by the existing hosting — nothing in the app or Play Console has been changed.
