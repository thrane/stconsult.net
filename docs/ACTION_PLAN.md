# Website Action Plan

Last updated: 2026-07-04

## Goal
Launch and iteratively improve the ST Consult website with clear, maintainable structure and truthful, high-signal content.

## Plan
1. Tailor homepage content to real profile and make it publish-ready.
2. Push repository and enable GitHub Pages deployment.
3. Add lightweight content update workflow for easier ongoing edits.

## Current Status
- Step 1: Complete
- Step 2: Complete
- Step 3: In progress — header, footer, and contact block are now shared via Jekyll includes, reducing duplicate edits across pages

## Step 1 Checklist
- Confirm public display name
- Confirm preferred contact email
- Confirm core services list
- Confirm CV source (link or 2-4 entries)
- Confirm optional links (LinkedIn/GitHub) — decided: LinkedIn link only, nothing worth showing on GitHub
- Update homepage copy in index.html
- Do final polish pass for clarity and consistency

## Notes
- 2026-07-04: Added technical SEO: `url`/`baseurl` and `jekyll-seo-tag`/`jekyll-sitemap` plugins in `_config.yml`, a shared `head-meta.html` include (SEO tag, favicon, Person JSON-LD), and `robots.txt`.
- 2026-07-04: Verified the site in Google Search Console and Bing Webmaster Tools, and submitted `sitemap.xml` to both.
- 2026-07-04: Updated the GitHub profile (`github.com/thrane`) website/social link to point to `stconsult.net` as an additional backlink; decided against adding a GitHub link on the site itself.
- 2026-07-04: Repository published to GitHub as `thrane/stconsult.net`, GitHub Pages enabled from `main`, custom domain `stconsult.net` connected, and HTTPS enforced.
- 2026-07-03: CV presented as external link instead of manual timeline entries.
- 2026-07-03: Replaced external CV link with internal `cv.html` summary page and added profile photo slot on homepage.
- 2026-07-03: Rewrote `cv.html` from a full career-history source into a short CV targeted at .NET lead-developer searches, limited to the last 10 years of projects, plus a separate skills section.
- 2026-07-03: Replaced the text brand with a logo image (`assets/Logo_black.png`), linked to the homepage.
- 2026-07-03: Introduced Jekyll to share header/footer/contact markup across pages and added a dedicated `contact.html` page; deploy workflow now builds with Jekyll before publishing.
