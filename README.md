# Shravani Patil — Portfolio

Source for [cluemore.github.io](https://cluemore.github.io), a recruiter-focused
portfolio for Data Science, Machine Learning, AI, and Analytics work.

This repository is being developed in small, working milestones. The current
milestone contains the global visual system, responsive editorial Hero, contact
links, accessibility foundations, and GitHub Pages deployment configuration.

## Technology

- Astro with static output
- TypeScript
- Plain CSS
- Locally bundled Instrument Serif and Inter fonts
- GitHub Pages through GitHub Actions

## Run locally

Requirements: Node.js 24 or newer.

```bash
npm install
npm run dev
```

Astro will print the local URL in the terminal.

## Validate a change

```bash
npm run check
npm run build
```

The static site is written to `dist/`.

## Common updates

- Profile and contact details: `src/data/profile.ts`
- Homepage composition: `src/pages/index.astro`
- Hero content and interaction: `src/components/Hero.astro`
- Contact section: `src/components/ContactStrip.astro`
- Global colours, typography, spacing, and responsive rules:
  `src/styles/global.css`
- Page metadata and shared document structure: `src/layouts/BaseLayout.astro`

## Deployment

The workflow at `.github/workflows/deploy.yml` builds and deploys every push to
`main`. In GitHub, the repository's **Settings → Pages → Source** must be set to
**GitHub Actions**.

The special repository name `cluemore.github.io` publishes at the root URL, so
the Astro configuration intentionally does not use a repository `base` path.

## Privacy

Only publication-ready content belongs in this repository. Do not commit API
keys, private contact data, unsanitised workplace screenshots, or `.env` files.

© Shravani Patil. All rights reserved.
