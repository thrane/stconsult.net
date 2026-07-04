# ST Consult Website

Simple static website for ST Consult, hosted on GitHub Pages.

## Current Stack
- HTML
- CSS
- Jekyll (for shared header/footer/contact includes; GitHub Pages builds this natively)
- GitHub Actions deployment to GitHub Pages

## Local Preview
Pages use Jekyll includes (`{% include %}`), so opening the HTML files directly in a
browser will show the raw tags instead of rendered content. To preview with includes
rendered:

```
bundle install
bundle exec jekyll serve
```

Then open the printed local URL (usually `http://127.0.0.1:4000`).

## Publish on GitHub Pages
1. Create a new GitHub repository and push this code to the `main` branch.
2. In GitHub, go to Settings -> Pages.
3. Under Build and deployment, select Source: GitHub Actions.
4. Push to `main` and wait for workflow `Deploy static site to GitHub Pages` to complete.

## Custom Domain Setup
This repo includes `CNAME` set to `stconsult.net`.

At your DNS provider, set:
- `A` records for apex domain (`stconsult.net`) pointing to GitHub Pages IPs:
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153
- `CNAME` record for `www` pointing to `<your-github-username>.github.io`

## Where To Edit Content
- Main content: `index.html`
- CV content: `cv.html`
- Contact details (shown on every page): `_includes/contact.html`
- Header/logo and footer (shared across pages): `_includes/header.html`, `_includes/footer.html`
- Visual design: `styles.css`
- Project rules/context: `docs/SITE_CHARTER.md`
- Content strategy: `docs/CONTENT_GUIDE.md`
