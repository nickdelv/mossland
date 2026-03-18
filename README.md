# Mossland

Brand and web design portfolio. Single-page static site.

**Live:** mossland.design
**Contact:** hello@mossland.design

---

## Structure

```
/
  index.html          — main page
  404.html            — custom not-found page
  CNAME               — custom domain for GitHub Pages
  robots.txt          — crawler directives
  sitemap.xml         — sitemap for search engines
  css/
    shared.css        — tokens, reset, shared components (footer, meta-loc, pills)
    index.css         — page-specific styles
    404.css           — page-specific styles for 404.html
  assets/
    favicon.svg       — primary favicon (modern browsers)
    favicon-32.png    — favicon fallback (32×32 PNG)
```

No build step. No framework. Deploy by pushing to host (Netlify, GitHub Pages, etc).

---

## Cache-busting

CSS files use query-string versioning: `?v=1.0`

Bump the version in the `<link>` tags in `index.html` when deploying visible style changes.

---

## Email

`hello@mossland.design` forwards to Gmail via Forwardemail.net (DNS MX records on Porkbun).
No Workspace required. Reply from Gmail using Send As alias.

---

## Fonts

Loaded via Google Fonts in `shared.css`:

- **Bebas Neue** — display / wordmark
- **Playfair Display** — headings, italic accents
- **EB Garamond** — body, labels, UI text

---

## Color tokens

| Token             | Value   | Use                         |
| ----------------- | ------- | --------------------------- |
| `--color-paper`   | #ede5cf | Page background             |
| `--color-ink`     | #150f08 | Primary text, dark sections |
| `--color-moss`    | #2b4816 | Accent, pills, links        |
| `--color-moss-lt` | #68a83e | Light accent (on dark bg)   |
| `--color-rule`    | #bfac88 | Borders, dividers           |
| `--color-muted`   | #6e6150 | Secondary text              |
