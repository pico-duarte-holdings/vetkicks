# VetKicks

Storefront for **VetKicks LLC** — veteran-owned sneaker resale in West Palm Beach, FL.
A Pico Duarte Holdings company.

**Live:** https://vetkicks.com

## What's here

| File | Page |
| --- | --- |
| `index.html` | Storefront — drops, the vault (filterable), legit-check protocol, contact form |
| `privacy.html` | Privacy policy |
| `terms.html` | Terms of service |
| `404.html` | Not-found page |
| `assets/` | Favicon and social share image |
| `CNAME` | Custom domain (vetkicks.com) |

Every page is a single self-contained HTML file — all styles, scripts, fonts and images
are embedded. No build step, no dependencies, no server. Open one in a browser and it works.

## Hosting

Served by GitHub Pages from the `main` branch, root folder.
`.nojekyll` is present so Pages serves the files as-is.

## Contact channel

There is no backend. The contact form and every "text to claim" button compose a
pre-filled SMS to **786-498-0991** and hand it to the visitor's messaging app
(on desktop, the message is copied to the clipboard instead). Nothing is submitted
to or stored on the site.

## Updating inventory

Inventory lives in the `items` array inside the inline script in `index.html`.
Each entry:

```js
{ name, brand, cw, size, cond, year, price, badge, featured, art }
```

- `badge`: `'HEAT'`, `'NEW'` or `''`
- `featured: true` puts the pair in the top "This week's heat" row
- `cond`: `DS`, `VNDS`, `USED 9/10`, `USED 8/10`
- `art`: the CSS gradient shown behind the emblem until real photos are added

---

© 2026 VetKicks LLC · Pico Duarte Holdings LLC
