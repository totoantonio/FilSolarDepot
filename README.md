# Fil Solar Depot Website

**DRAFT** (yellow banner fixed at the top inside the header; remove the `.draft` div before launch).

Website for Fil Solar Depot, backed by HE & SONS (Chevron Lubricants distributor).

- **Live:** https://totoantonio.github.io/FilSolarDepot/
- **Repo:** https://github.com/totoantonio/FilSolarDepot
- **Credit:** totoantonio.cloud (hidden in page meta)

## Stack
One `index.html` (styles + script inside) and `images/`. No framework, no build step. Font: Plus Jakarta Sans (Google Fonts).

## Files
- `index.html` — the whole site
- `images/logo.png` — Fil Solar Depot logo, transparent background (white removed 2026-10-24)
- `images/og.png` — 1200×630 share preview image
- `images/tesda.svg` — TESDA seal (Wikimedia Commons)
- `images/*-625.png`, `jinko-590.png`, `hestia-650.png`, `rail.png` — product photos cropped from screenshots (replace with originals)

## Preview and publish
- Preview: `open index.html`
- Publish: commit and push to `main`; GitHub Pages rebuilds in about a minute.
- Facebook link preview cached? Use developers.facebook.com/tools/debug → Scrape Again.

## Page sections
Product-focused layout (since 2026-10-24). Old layout saved as git tag `v1-before-product-site` (restore: `git checkout v1-before-product-site -- index.html`).

0. Yellow DRAFT banner, stays fixed with the menu while scrolling (remove before launch)
1. Hero: animated house ↔ HE & SONS building; Order Now / View Products
2. Figures strip (navy gradient)
3. Explore Our Solar Panels: 4 perks + 4 large tinted product cards (spec line, price, Order Now, Specifications panel)
4. Why Fil Solar Depot? (8 tinted cards, one-line titles)
5. Our Story (facts card stays in view while the story scrolls)
6. Place Your Order → Order Summary pop-up (order no., Save as PDF / Print) → GCash/QR Ph or Bank Transfer
7. Testimonials (SAMPLE, swipe row on phones)
8. FAQ (rounded question boxes)
9. Footer (navy gradient); phone bottom bar (View Products / Order Now)

Style: Google Home–inspired. Logo colors only: orange→red gradient (`--sun`) for highlights and main buttons, navy/blue for text and outlines, light tints `--tint-sun` / `--tint-blue` for cards. Every section heading = small orange label + large navy title with one gradient word. Content fades up on scroll; soft glows drift behind Products and Why Us. Savings calculator removed.

## Still placeholder (yellow highlight or noted in code)
- Product prices (`data-price` + ₱ text in the order form; "Price TBA" on cards)
- Battery and inverter models
- Mounting rail specs
- Contact: phone, email, address, hours (footer)
- Bank details and GCash/QR Ph code
- Payment-proof email `PAY_EMAIL` (given as admin.lloyd@he@sons.com, which is invalid; using admin.lloyd@heandsons.com)
- Formspree ID `YOUR_FORM_ID` (order + consultation forms) — until set, orders show "couldn't send, email the PDF"
- Installation partner website link (service card 4 + FAQ, `href="#"`)
- Calculator assumptions: ₱12/kWh, ₱50,000/kWp installed
- Testimonials are SAMPLES — replace with real reviews (with permission)
- Confirm services offered (net metering help, delivery, warranty support, maintenance)
- Small square favicon

## SEO / AI visibility
- `llms.txt` (summary for ChatGPT, Claude, Perplexity), `robots.txt` (all search and AI bots allowed), `sitemap.xml`
- Structured data (JSON-LD) in `<head>`: business profile + FAQ; geo tags for Cagayan de Oro
- On github.io, robots.txt and llms.txt only count at the domain root, so they take full effect after moving to a custom domain. Until then, submit `sitemap.xml` in Google Search Console and Bing Webmaster Tools
- Keep llms.txt and JSON-LD in sync when contact details, products or FAQ change
