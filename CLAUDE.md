# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Rules

- When encountering author names that use only a first initial (e.g., "C. A. Hadar", "K. Gruteke Klein"), always ask the user for the full first name. Do not guess or assume what the initial stands for.

## Architecture

Plain HTML + CSS personal academic website adapted from a public academic homepage template. Deployed to GitHub Pages via GitHub Actions in `.github/workflows/jekyll-gh-pages.yml`.

No build step required. The site is a single `index.html` file with a `stylesheet.css`.

### Key Files

- `index.html` — The homepage content and metadata
- `stylesheet.css` — Layout, typography, color tokens, and responsive styling
- `images/` — Optional site assets such as a profile photo
- `data/` — Optional local PDFs and supporting files
- `.github/workflows/jekyll-gh-pages.yml` — GitHub Actions workflow for static site deployment

### Content Sections (in index.html)

1. Header and profile summary
2. Research focus
3. Selected publications
4. Community and affiliation

### Adding a New Publication

Add a new `article.publication-item` block inside the `publication-list` container in `index.html`.

- Update the year and venue pills in `pub-meta`
- Keep author formatting consistent across entries
- Add links only for pages that are publicly available
- Preserve the two-column publication card structure for desktop and stacked layout for mobile

### Deployment

Push to `main` triggers GitHub Actions which deploys the root directory as a static site to GitHub Pages. No build step needed.
