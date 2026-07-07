# Longboard® — interim site (V1)

Single-page static site for Longboard Architectural Products. No build step,
no dependencies, no backend — one HTML file, five images, a favicon.

## Deploy on GitHub Pages

1. Push this folder's contents to a repo (root, or `/docs`).
2. Repo → Settings → Pages → Source: **Deploy from a branch** → select the
   branch (and `/ (root)` or `/docs`).
3. The site is live at `https://<user>.github.io/<repo>/` within a minute.
4. Custom domain: add it under Settings → Pages and point the client's DNS
   (CNAME for `www`, A/ALIAS for apex) when ready.

Works identically on Netlify / Vercel / S3 — drop the folder, done.

## Before pointing real traffic at it

- Set the `og:image` meta tag in `index.html` to an absolute URL once the
  final domain is known (line is marked with a TODO comment).
- Confirm contact routing: the page uses `tel:1-800-604-0343` and
  `mailto:info@longboardproducts.com`.

## Files

```
index.html      the site
assets/         5 images (compressed for web)
favicon.svg
404.html        redirects to /
```
