# Zeaj Zamoranos — Portfolio

Static site (HTML/CSS/JS, no build step) built from the Figma file *Zeaj's Portfolio → Draft v2 → Home / Template*.

## Preview locally
```bash
python3 -m http.server 4173 --bind 127.0.0.1
```
Then open http://localhost:4173.

## Edit your links
All links (LinkedIn, GitHub, résumé, email, case-study pages) live in `js/config.js`.
Empty values stay inert until filled in. The email is stored in two halves and only assembled on click.

## Breakpoints
| Name | Width | Layout |
|---|---|---|
| Desktop | ≥1200px | 300px sticky sidebar, content capped at 1440px |
| Tablet | 810–1199px | 220px sidebar, tighter padding |
| Mobile | <810px | Top bar + full-screen menu, one-column cards |

## Security
- Strict Content-Security-Policy (no inline scripts/styles, no third-party scripts, no network calls from the page).
- Hosting headers in `vercel.json` (Vercel) and `_headers` (Netlify / Cloudflare Pages): HSTS, no framing, nosniff, strict referrer, locked-down permissions.
- External links open with `rel="noopener noreferrer"`; config URLs are restricted to `https://` or same-site paths.
- No analytics or trackers. Theme choice is the only thing stored (in the visitor's own browser).
- Before adding photos or a résumé: export fresh copies so phone GPS/camera metadata and personal details (phone, address) aren't published.

## Deploy
Push this folder to a GitHub repo and import it in Vercel or Netlify (framework: "Other", no build command, output = repo root).
