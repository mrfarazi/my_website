# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal academic website for Moshiur Farazi (AI & Computer Vision researcher, Assistant Professor at UDST). Static site with no build system, package manager, or framework.

## Architecture

- **index.html** — Main landing page (bio, news, selected publications)
- **cv.html** — CV / resume page
- **publications.html** — Full publications list
- **assets/css/style.css** — All styles (shared across pages)
- **assets/js/main.js** — Minimal JS (hamburger menu, mobile nav)

All pages share a common sidebar layout with responsive mobile header. Fonts are loaded from Google Fonts (Source Serif 4, Inter).

## Development

No build step. Open any HTML file directly in a browser or use a local server:

```
python3 -m http.server 8000
```

## Notes

- Pages use a two-column layout: fixed sidebar + scrollable main content
- Navigation between pages is plain `<a>` links — keep nav consistent across all HTML files when adding/removing pages
