# BezVox Website

Static marketing website for **BezVox**, a communications company offering temporary staffing services to local businesses.

- **Address:** 30201 Orchard Lake Rd, Farmington Hills, MI 48334
- **Domain:** [bezvox.com](https://bezvox.com)
- **Hosting:** GitHub Pages (deployed automatically via GitHub Actions on every push to `main`)

## Structure

- `index.html` — single-page site (hero, services, about, contact)
- `assets/styles.css` — site styles
- `CNAME` — custom domain for GitHub Pages
- `.github/workflows/deploy-pages.yml` — Pages deployment workflow

## Custom domain setup

1. In the repo: **Settings → Pages → Custom domain** → enter `bezvox.com` and save.
2. At your DNS provider for `bezvox.com`, add:
   - Four `A` records for the apex (`@`): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - A `CNAME` record for `www` → `mmbezalu.github.io`
3. Back in **Settings → Pages**, enable **Enforce HTTPS** once the certificate is issued.
