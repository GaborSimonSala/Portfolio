# Portfolio

A modern, single‑page personal portfolio website for showcasing experience, skills, and selected projects. The site is built with plain HTML, CSS, and vanilla JavaScript and is designed to be easily hosted on any static hosting provider (e.g., GitHub Pages, Netlify, Vercel, or a simple web server).

## Overview
- Tech stack: HTML5, CSS3, Vanilla JavaScript
- No build step, no package manager, no server‑side backend
- Entry point: `index.html`
- Styling: `styles.css`
- Client logic and interactions: `script.js`
- External CDNs:
  - Font Awesome (icons)
  - Google Fonts (Inter, Poppins)

Sections included:
- Navigation with smooth scrolling and active‑link highlighting
- Hero with optional typing and parallax effects (WIP)
- About with stats (WIP)
- Experience timeline (WIP)
- Skills with animated progress bars (WIP)
- Project examples (WIP)
- Contact form (WIP)
- Footer with social links (WIP)

## Requirements
- A modern web browser (Chrome, Firefox, Edge, Safari)

## Getting Started (Run Locally)
You have two easy options:

1) Open directly in a browser
- Double‑click `index.html` to open it in your default browser.
- Note: Some features work best when served over HTTP rather than via the `file://` protocol.

2) Serve via a simple local server (recommended)
- VS Code extension: "Live Server" → Right‑click `index.html` → "Open with Live Server".
- Python 3 (if installed):
  - PowerShell: `python -m http.server 8000`
  - Then open: http://localhost:8000/
- Node.js http-server (if installed):
  - `npx http-server -p 8000`
  - Then open: http://localhost:8000/

## Scripts
There is no package.json and no NPM/Yarn/PNPM scripts in this repository. All behavior is handled by `script.js` and runs in the browser.

## Environment Variables
None are required.

## Tests
There are currently no automated tests in this repository.

## Project Structure
```
Portfolio/
├─ index.html      # Main HTML entry point
├─ styles.css      # Global styles
├─ script.js       # Client‑side interactivity and animations
└─ README.md       # This documentation
```

## Notable Implementation Details
- Smooth scrolling and active section highlighting are implemented in `script.js`.
- IntersectionObserver is used to trigger reveal animations and skill bar animations.
- Contact form (`#contactForm`) performs basic validation and then simulates an async submit with a loading state and success alert.
- The navbar updates style on scroll.
- Google Fonts and Font Awesome are loaded via CDN in `index.html`.

## Deployment
Because this is a static site, deployment is simple:
- GitHub Pages: Push to a public repository and enable Pages → set root to the main branch.
- Netlify: Drag and drop the folder or connect the repository; publish directory is the repo root.
- Vercel: Import the repository; set framework to "Other" and output directory to the repo root.
- Any static web server: Serve the repository root so `index.html` is accessible at `/`.

## Accessibility & SEO (TODO)
- Ensure alt text for images (the demo sticker image includes alt text).
- Consider adding meta description and Open Graph tags.
- Verify color contrast in `styles.css` if you customize the palette.

## License
This project is licensed under the Gábor Simon Proprietary License — see the [LICENSE](LICENSE) file for details. You may not modify or redistribute any part of this software without the prior public written permission of the copyright holder. For permission requests, please reach out via the Contact section of this site (see the Contact section in index.html).

© 2025 Gábor Simon