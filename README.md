# Personal Website

A modern personal website built with vanilla JavaScript and Vite.

## Project Structure

```
├── src/
│   ├── styles/
│   │   ├── reset.css          # CSS reset
│   │   ├── variables.css      # Design tokens from Figma
│   │   ├── main.css          # Main styles
│   │   └── components/       # Component-specific styles
│   ├── js/
│   │   ├── main.js           # JavaScript entry point
│   │   └── components/       # JavaScript components
│   └── assets/
│       ├── images/           # Images
│       └── fonts/            # Custom fonts
├── public/                   # Static assets
├── index.html               # Main HTML file
└── package.json

```

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Design Tokens

All design tokens (colors, typography, spacing) are centralized in `src/styles/variables.css`.
Update these values based on your Figma designs.

## Deployment

This site can be deployed to:
- Vercel (recommended)
- Netlify
- GitHub Pages
- Cloudflare Pages

See deployment instructions in the main documentation.
