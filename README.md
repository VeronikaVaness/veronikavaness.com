# Veronika Vaness — Artist Website

The personal website for watercolour artist Veronika Vaness — portfolio, about, and commissions.
Static HTML/CSS, hosted on **GitHub Pages**, domain managed by **Cloudflare** (`veronikavaness.com`).

## Structure

```
index.html          Home
gallery.html        Gallery / portfolio
about.html          About + process
commissions.html    Commissions & contact
404.html            Friendly not-found page
favicon.svg         Site icon
CNAME               Custom domain for GitHub Pages
assets/
  css/style.css     All site styling (the "Ink & wash" brand system)
  img/              Web-optimized artwork + og-image (these ARE published)
01 Collection/      High-res source artwork (LOCAL ONLY — git-ignored)
```

## Editing

- All visual styling lives in `assets/css/style.css` (colours and fonts are CSS variables at the top).
- To add a painting: drop the web-optimized image in `assets/img/`, then copy a `<figure class="piece">` block in `gallery.html`.
- New artwork should be ~1600px on the long edge, JPEG quality ~82, EXIF-rotated. (Claude handles this automatically.)

## Placeholders to replace before/after launch

- **Painting titles, sizes, editions, and prices** — currently working titles.
- **Email** `hello@veronikavaness.com` — set up email (e.g. Cloudflare Email Routing) so it forwards to a real inbox.
- **About photo** — optional: add a real portrait of Veronika.

## How deployment works

1. Site files live in this repo.
2. Pushing to the `main` branch updates GitHub Pages automatically (usually live within a minute).
3. Cloudflare DNS points `veronikavaness.com` at GitHub Pages.

## Brand

Colours, type, voice, and usage rules are in the Brand Guidelines (kept locally, not published).
Palette: Paper `#F6F5F1` · Ink `#25303B` · Indigo `#4C6B8A` · Taupe `#C9BBA8` · Terracotta `#CC7357`.
Type: Playfair Display (headings) + Inter (body).
