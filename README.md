# mekriva-web

Landing page for [Mekriva](https://mekriva.com) — a small engineering team based in Seville, Spain, specializing in embedded systems, IoT, custom hardware, and cloud software.

## Stack

Single-file static site (`index.html`). No build step, no dependencies — just HTML, CSS, and vanilla JS.

- **Fonts**: Space Grotesk via Google Fonts
- **Icons**: Font Awesome 6.5.0 (free CDN)
- **Forms**: [Formspree](https://formspree.io) (endpoint not yet configured — see comment in the HTML)
- **i18n**: Built-in EN/ES toggle, persisted in `localStorage`

## Development

Open `index.html` in a browser directly, or serve it locally:

```bash
npx serve .
# or
python3 -m http.server
```

## Deployment

Static file — deploy anywhere: GitHub Pages, Netlify, Vercel, Cloudflare Pages, etc.

## Contact

hellothere@mekriva.com
