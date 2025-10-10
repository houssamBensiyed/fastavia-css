# Festava Live — Static CSS Website

This repository contains a small static website for the "Festava Live" music festival. It's a plain HTML/CSS project (no build step) intended as a theme / landing site for a festival, with pages for tickets, artists, schedule, pricing, contact, etc.

## What's in this repo

Top-level files:

- `index.html` — Home / landing page
- `about.html` — About the festival
- `artists.html` — Artists / performers
- `schedule.html` — Event schedule
- `pricing.html` — Pricing details
- `ticket.html` — Ticket purchase page (detailed form)
- `contact.html` — Contact information

Directories:

- `css/` — All CSS files used by the site (Bootstrap + custom styles)
  - `bootstrap.min.css`, `bootstrap-icons.css`, `styles.css`, `templatemo-festava-live.css`
- `js/` — JavaScript files (vanilla helpers and jQuery)
  - `jquery.min.js`, `bootstrap.min.js`, `custom.js`, `jquery.sticky.js`
- `fonts/` — Custom fonts used by the site
- `images/` — All images (including `images/artists/`)
- `video/` — Example video assets

## Features

- Fully static site using HTML, CSS and light JavaScript.
- Responsive layout with mobile-friendly breakpoints.
- Ticket purchase page (`ticket.html`) with a styled form and order summary.
- Uses Bootstrap for base layout and utility classes plus custom theme CSS.

## How to preview locally

Because this is a static site you can preview it in any browser. A few recommended ways:

- Open `index.html` directly in your browser (double-click or use the OS "Open with" option).

- From Visual Studio Code: install the "Live Server" extension, open the repo, then click "Go Live" to serve and preview with auto-reload.

- From a simple local HTTP server (PowerShell / Command Prompt):

```powershell
# If you have Python 3 installed (recommended), run from the repo root:
py -3 -m http.server 8000
# or (if 'py' is not available):
python -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## Development notes

- CSS lives in `css/`. `styles.css` is the main custom stylesheet — edit it for visual changes.
- JavaScript hooks are in `js/custom.js`. Minimal behavior (sticky nav, small interactions) is implemented there.
- Images and media are stored in `images/` and `video/` respectively.
- Pages are plain HTML files; to add a page copy an existing file (for example `about.html`) and update the markup and navigation links.

## Adding or editing content

- Update the HTML file for page content.
- Update `css/styles.css` for custom layout or theme changes.
- Add images to `images/` and reference them with the relative path from the HTML file.

## Accessibility & performance tips

- Keep images optimized for web (compressed JPEG/PNG or modern formats like WebP).
- Add alt attributes to images for accessibility.
- Minify CSS/JS for production if serving on a public site.

## Live deployment

Since this is static, you can host it on any static hosting service (GitHub Pages, Netlify, Vercel, S3, etc.). For GitHub Pages, push to a GitHub repo and enable Pages from the repository settings (use the `gh-pages` branch or the `main` branch root).

## Contributing

This repo is currently a simple static site. To contribute:

1. Fork the repository.
2. Make your changes on a branch.
3. Submit a pull request describing your changes.

If you want help improving the site (layout, accessibility, or converting to a build system like a static site generator), open an issue describing what you want to do.

For questions about this repository, update requests, or help converting it into a larger project, open an issue in the repository or reach out to the maintainer.
