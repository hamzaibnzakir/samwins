# Samwins Mentorship — landing page

Static landing page for **Samwins Mentorship** (1-on-1 ecommerce mentorship).

- `index.html` — the whole page (HTML + CSS + JS in one file, motion built with anime.js 3.2.2)
- `assets/proof/` — student result screenshots (`-sm` = grid thumbnails, full size for the lightbox)
- `assets/video/` — order-feed video + poster
- `assets/brand/` — logo (SVG/PNG), favicons, social share image (`og.png`)

## Features
- Multi-step **Apply** popup → submits to Formspree (`https://formspree.io/f/xzedealb`)
- Floating **WhatsApp** quick-contact button (+1 646 918 3126)
- Filterable results wall with lightbox, auto-playing order video
- TikTok + Instagram social cards with a spinning "Follow the wins" badge and a side rail on wide screens

## Editing results
Add a screenshot as `assets/proof/proof-17.webp` (+ `proof-17-sm.webp`), then add a line to the `PROOF` array in `index.html`:
```js
{n:17, t:"$9,420", s:"Sales in one day · 140 orders", f:"day", tag:"One day"},
```
`f` is the filter: `week`, `day` or `milestone`.

## Deploy
No build step. Import the repo on Vercel/Netlify (framework: "Other") or enable GitHub Pages on `main`.
