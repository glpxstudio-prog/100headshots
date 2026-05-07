# 100headshots.com

Public landing page for the GLPX Studio **$100 Headshots Limited Release** — a capped Orlando promotion (15-min studio session, 1 retouched final, $50 deposit + $50 day-of, capped at 100 spots).

Hosted on GitHub Pages, custom domain `100headshots.com`.

## Stack

- Single static HTML (`index.html`) — Tailwind CSS via CDN, Google Fonts, vanilla JS
- GHL booking calendar embedded via iframe (id `lKRCEn1Q3E2jWf9yuKA3`)
- Stripe $50 deposit collected by GHL
- Meta Pixel `1140403037921588` (PageView + Schedule events)
- Schema.org JSON-LD (LocalBusiness + Offer + FAQPage)
- Asset images in `100-headshots-assets/`

## Updating

1. Edit `index.html` directly
2. Update `SPOTS_REMAINING` constant in the `<script>` block as bookings come in (manual — no fake countdowns, FTC compliance)
3. `git push` — GitHub Pages auto-deploys on push to `main`

## DNS for `100headshots.com`

```
Type   Name   Value
A      @      185.199.108.153
A      @      185.199.109.153
A      @      185.199.110.153
A      @      185.199.111.153
CNAME  www    glpxstudio-prog.github.io
```

In GitHub repo Settings → Pages, confirm the custom domain and enable HTTPS.
