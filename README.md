# LittleDays — landing / waitlist site

A single static page (`index.html`) for the LittleDays waitlist, matched to the
app's brand. Built to capitalize on the TikTok traffic while the app is in App
Review. Deploys on GitHub Pages — no build step.

## To go live (≈5 min)

### 1. Wire up the email capture (ConvertKit)
1. Make a free ConvertKit account → **Grow → Landing Pages & Forms → New → Form → Inline**.
2. Click **Embed → HTML** and copy the `<form action="...">` URL. It looks like
   `https://app.kit.com/forms/1234567/subscriptions`.
3. In `index.html`, find `REPLACE_WITH_CONVERTKIT_FORM_ACTION_URL` and paste that
   URL in. That's the only edit needed. (Until then the page works as a teaser —
   the success message still shows for testing.)
4. At launch, send the "we're live" broadcast to the form's subscribers from
   ConvertKit in one click.

### 2. Publish on GitHub Pages
```bash
# from this folder
git init && git add -A && git commit -m "LittleDays waitlist landing page"
gh repo create little-days-site --public --source=. --push
```
Then on GitHub: **Settings → Pages → Source: `main` / root**. The site goes live
at `https://lhakso.github.io/little-days-site/` — that's the bio link.

### 3. (Optional) Custom domain
Add a `CNAME` file containing your domain (e.g. `littledays.app`), point the
domain's DNS at GitHub Pages, and enable it under Settings → Pages.

## Notes
- `logo.png` — app icon (rounded square), used as the hero mark + favicon.
- `logo-flower.png` — transparent sunflower mark, used as the social-share image.
- Palette and serif font are pulled straight from the iOS app's `Theme.swift`
  and the privacy site, so it feels like the same product.
