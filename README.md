# MedCollect — Landing Page

Marketing landing page for MedCollect (precision medical billing & revenue cycle management for healthcare providers).

This is a single, self-contained static site — everything lives in `index.html`, with no build step or dependencies to install.

## Deployment

The site is hosted on **GitHub Pages**, served from the `main` branch (root).

- **Custom domain:** `medcollect.com` — set via the `CNAME` file in this repo plus DNS records at the domain registrar (GoDaddy).
- **HTTPS:** provisioned automatically by GitHub Pages (Let's Encrypt).
- **Jekyll:** disabled via the `.nojekyll` file so the static files are served exactly as-is.

### DNS records (set at the registrar)

For the apex domain `medcollect.com` — four `A` records:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

For `www.medcollect.com` — one `CNAME` record pointing to `rhythmmittal19.github.io`.

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.
