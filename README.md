# shir-lissak.github.io

Academic homepage for Shir Lissak, adapted from a public academic GitHub Pages template into a simpler static one-page profile.

## Structure

This repo is plain HTML and CSS. There is no local build step.

- `index.html` - homepage content, metadata, and section structure
- `stylesheet.css` - layout, typography, colors, and responsive styling
- `images/` - optional site assets if a profile image or thumbnails are added later
- `.github/workflows/jekyll-gh-pages.yml` - GitHub Pages deployment workflow

## Running locally

Open `index.html` directly in a browser, or serve the folder with any static file server.

## Publishing as your own repo

This workspace was cloned from the source template repository, so you should attach it to your own GitHub repository before pushing.

Example:

```powershell
git remote rename origin upstream
git remote add origin https://github.com/<your-user>/<your-repo>.git
git push -u origin main
```

## Notes

- The page content was initialized from publicly available profile and publication references.
- The site is ready for further refinement with a profile image, additional publications, talks, or a CV link.
