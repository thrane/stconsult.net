# ST Consult Website Charter

## Purpose
This repository contains the public website for ST Consult (stconsult.net).

The website should communicate:
- Who I am
- What I do
- How to contact me
- Why clients can trust my software delivery quality

## Non-Negotiable Quality Principles
These principles are tool- and agent-agnostic. Any contributor (human or AI) must follow them.

1. Keep it maintainable:
- Prefer simple structure over cleverness.
- Keep files small and responsibilities clear.
- Avoid unnecessary frameworks until they solve a real problem.

2. Preserve quality:
- Changes should be readable and easy to review.
- Avoid duplicate content and duplicated styling logic.
- Remove dead code and outdated text.

3. Keep content truthful and current:
- Do not exaggerate skills, roles, or project outcomes.
- If a claim cannot be verified, rewrite or remove it.
- Prefer specific facts over vague buzzwords.

4. Optimize for iteration:
- Every section should be easy to edit by hand.
- Content updates should not require redesign.
- Introduce complexity only when needed.

5. Keep performance and accessibility in scope:
- Fast loading first.
- Semantic HTML where possible.
- Sufficient color contrast and keyboard-friendly interactions.

## Technical Direction (Current)
- Hosting: GitHub Pages
- Stack: Static HTML + CSS, with Jekyll for shared includes (header, footer, contact block) — built natively by GitHub Pages
- Domain: stconsult.net

## Initial Content Scope (MVP)
- Hero/introduction
- Contact information
- Short CV / selected experience timeline
- Optional short list of services

## Decision Log
Record important architectural or content decisions here as they happen.

- 2026-07-03: Start with static HTML/CSS for fast launch and low maintenance.
- 2026-07-03: Rewrote `cv.html` as a short CV targeted at teams looking for a lead developer on a .NET project, sourced from a full career-history document and scoped to the last 10 years of projects; added a separate "Core skills (last 7 years)" section.
- 2026-07-03: Adopted Jekyll (native GitHub Pages support) to share header, footer, and contact markup across pages via `_includes/`, added a dedicated `contact.html` page, and updated the deploy workflow to build with Jekyll before publishing. `docs/` and `README.md` are now excluded from the published output.
- 2026-07-03: Replaced the text brand mark with the `Logo_black.png` logo in the header, linked to the homepage.
- 2026-07-03: Decided against offering a downloadable full-length CV. Kept "full details available on request" as an email-gated ask instead — preserves engagement and lets the CV be tailored per opportunity rather than commoditized as a static download.

## Change Checklist
Before merging any change:
- Does this keep the site easy to maintain?
- Is the content accurate and up to date?
- Is the visual result readable on mobile and desktop?
- Does this add complexity without clear benefit?
