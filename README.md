# Patrick Stewart — Personal Website

Personal portfolio site for Patrick Stewart, Technical Product Manager.

## Stack

- Vanilla HTML/CSS/JS
- [Vite](https://vitejs.dev/) (via rolldown-vite)
- Deployed on [Vercel](https://vercel.com)

## Development

```bash
npm install
npm run dev      # Start dev server with hot reload
npm run build    # Build to /dist
npm run preview  # Preview production build locally
```

## Structure

```
index.html          # All page content (single page)
src/
  main.js           # Entry point — imports CSS
  styles/
    variables.css   # Design tokens (colours, fonts, spacing)
    main.css        # All component styles
    reset.css       # Base reset
public/
  images/           # Article images, profile photo, favicon
  cv/               # CV PDF
```

## Design

Dark theme with gold accent (`#c8b88a`). Fonts: DM Serif Display (headings) + DM Sans (body). All design values are CSS custom properties in `src/styles/variables.css`.

## Figma

Design file: [Personal Website Revamp](https://www.figma.com/design/B5jQazlCEsZdyt0oH7KFs1/Personal-Website-Revamp)
