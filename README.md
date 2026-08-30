# LittleDays — landing site

A single static page (`index.html`) for LittleDays, matched to the app's brand.
Deploys on GitHub Pages — no build step. Live at
[littledaysfamily.com](https://littledaysfamily.com/) (see `CNAME`).

The page points at the App Store listing:
`https://apps.apple.com/us/app/littledaysfamily/id6761935976`

## Editing
Everything is in `index.html` — markup and styles in one file, no JS.
Push to `main` and GitHub Pages redeploys.

## Notes
- `logo.png` — app icon (rounded square), used as the hero mark + favicon.
- `logo-flower.png` — transparent sunflower mark.
- `og-image.png` — social share card (1200×630).
- `shots/` — framed product screenshots.
- Palette and serif font are pulled straight from the iOS app's `Theme.swift`
  and the privacy site, so it feels like the same product.
