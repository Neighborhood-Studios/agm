# Neighborhood Studios — AGM (Friday) · static site

Self-contained static site for the Neighborhood Studios Annual General Meeting (Friday-only version). Deploys as-is to GitHub Pages or any static host.

## Files
- `index.html` — the page (entry point)
- `styles.css` — brand stylesheet (imports Google Fonts + the token files)
- `tokens/` — CSS custom properties (colors, type, spacing, effects, base)
- `assets/logos/` — wordmark + knot mark
- `assets/images/` — event + Fund 1 photos (web-optimized) and easter-egg stickers

All asset paths are relative (`./assets/...`), so the folder works from any subpath.

## Deploy to GitHub Pages
1. Put the **contents of this folder** at the repo root (or in `/docs`).
2. Repo → **Settings → Pages** → Source: `main` branch, root (or `/docs`).
3. The site is live at `https://<user>.github.io/<repo>/`.

Or drag-drop the folder into Netlify / Cloudflare Pages / Vercel — no build step.

## Notes
- Fonts load from Google Fonts over the network (needs internet at view time).
- Photos were downscaled to ~1600px / JPEG q82 for fast loading.
- Tested: no console errors, no horizontal overflow, mobile-responsive.
