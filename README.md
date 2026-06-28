# Mekriva Web

Landing page for [Mekriva](https://mekriva.com) — an engineering studio based in Seville, Spain, specialising in embedded systems, IoT, custom hardware, and cloud software.

## Stack

Single-file static site. No build step, no framework, no dependencies.

- **HTML/CSS/JS** — vanilla, zero tooling required
- **Fonts** — Space Grotesk via Google Fonts
- **Icons** — Font Awesome 6.5 (free CDN)
- **Forms** — [Web3Forms](https://web3forms.com) (contact form submission)
- **i18n** — built-in EN/ES toggle, persisted in `localStorage`
- **Hosting** — GitHub Pages (custom domain via `CNAME`)

## Files

```
index.html                  Main landing page (single-page, anchor navigation)
aviso-legal.html            Legal notice (LSSI-CE art. 10)
politica-de-privacidad.html Privacy policy (RGPD + LOPDGDD)
sitemap.xml                 XML sitemap for search engines
robots.txt                  Crawler directives
logo.png                    Favicon / brand logo
CNAME                       GitHub Pages custom domain (mekriva.com)
```

## Local development

Open `index.html` directly in a browser, or serve locally to avoid CORS issues:

```bash
npx serve .
# or
python3 -m http.server
```

## SEO

- `<title>` and `<meta description>` are keyword-optimised for embedded systems / IoT / Spain
- Open Graph and Twitter Card meta tags for social sharing
- `hreflang` alternates for EN and ES (both served at the same URL)
- JSON-LD structured data (`ProfessionalService` schema)
- `sitemap.xml` submitted to Google Search Console
- Legal pages use `noindex` to avoid competing with the homepage

## Accessibility

- Skip-to-content link (visible on focus)
- `<main>` landmark wrapping all page sections
- `<nav aria-label>` on primary navigation
- Hamburger converted to `<button>` with `aria-expanded` / `aria-controls`
- Language toggle uses `<button role>` with `aria-pressed`
- All form inputs have programmatically linked `<label for>` + `id`
- `autocomplete` attributes on contact form fields
- Decorative icons marked `aria-hidden="true"`

## Deployment

Push to `main` — GitHub Pages deploys automatically.

## Contact

hellothere@mekriva.com
