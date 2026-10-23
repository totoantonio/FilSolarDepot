# Fil Solar Depot Website

Website for Fil Solar Depot, backed by HE & SONS (Chevron Lubricants distributor).

- **Live:** https://totoantonio.github.io/websiteproject/
- **Repo:** https://github.com/totoantonio/websiteproject
- **Credit:** totoantonio.cloud (hidden in page meta)

## Stack
One `index.html` (styles + script inside) and `images/`. No framework, no build step. Font: Google Sans.

## Files
- `index.html` — the whole site
- `images/logo.png` — Fil Solar Depot logo
- `images/og.png` — 1200×630 share preview image
- `images/tesda.svg` — TESDA seal (Wikimedia Commons)
- `images/*-625.png`, `jinko-590.png`, `hestia-650.png`, `rail.png` — product photos cropped from screenshots (replace with originals)

## Preview and publish
- Preview: `open index.html`
- Publish: commit and push to `main`; GitHub Pages rebuilds in about a minute.
- Facebook link preview cached? Use developers.facebook.com/tools/debug → Scrape Again.

## Page sections
1. Hero: animated house ↔ HE & SONS building, panels drop in, sun arcs, crew working; fills the first screen
2. Figures strip
3. Savings calculator (pop-up) → Book a Free Consultation form
4. Why Fil Solar Depot? (8 service cards, Apple-style reveal)
5. Why Our Panels
6. Products (specs expand per card)
7. Our Story (50 years in business, TESDA-trained team, warranty seal)
8. Order Form → Place Order → Order Summary pop-up (order no., Save as PDF / Print) → GCash/QR Ph or Bank Transfer
9. Testimonials (SAMPLE, swipe row on phones)
10. FAQ
11. Footer (contact, quick links); phone bottom bar (Calculate Savings / Get a Free Quote)

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
