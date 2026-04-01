# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # Start local dev server (Vite, hot reload)
npm run build    # Build to /dist
npm run preview  # Preview the production build locally
```

## Architecture

Single-page personal portfolio site. No framework — vanilla HTML, CSS, and JS bundled with Vite.

**Entry points:**
- [index.html](index.html) — entire page markup (one file, all sections inline)
- [src/main.js](src/main.js) — JS entry point; currently only imports CSS
- [src/styles/main.css](src/styles/main.css) — all component and section styles
- [src/styles/variables.css](src/styles/variables.css) — all design tokens (colours, fonts, spacing, radii, transitions)
- [src/styles/reset.css](src/styles/reset.css) — base reset

**Static assets** live in [public/](public/) and are served at the root:
- `public/images/` — article images, profile photo (`profile.jpg`), favicon
- `public/cv/` — downloadable CV PDF

**Layout structure** (in order in `index.html`):
`nav` → `#hero` → skills-strip → `#work` (cards) → `#career` (timeline) → `#writing` (article cards) → `#contact` → `footer`

Nav links are in-page anchor links (`#work`, `#career`, `#writing`, `#contact`).

## Design tokens

All visual values are CSS custom properties defined in [variables.css](src/styles/variables.css). Always use these — never hardcode colours, radii, or transitions.

Key tokens:
- `--color-bg: #0d0d0d` / `--color-accent: #c8b88a` (gold)
- `--font-serif: 'DM Serif Display'` (headings) / `--font-sans: 'DM Sans'` (body)
- `--content-max: 796px` — max content width
- `--content-offset: 358px` — used for asymmetric section layouts

## Deployment

Deployed on Vercel. `vercel.json` sets `cleanUrls: true`. Pushing to `main` triggers a deploy.
