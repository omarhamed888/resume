# Omar Hamed Ali — Portfolio

Personal portfolio / résumé site for **Omar Hamed Ali**, AI Engineer & Data Scientist.

**Live:** https://omarhamed888.github.io/resume/

## About

A single-page portfolio covering experience, AI/ML and Data/BI projects, verified
certifications, skills, and contact channels. Built as one self-contained `index.html`
(no build step) with a light/dark theme, responsive layout, scroll animations, and an
accessible image lightbox.

## Tech

- Hand-written HTML, CSS (custom design tokens, dual theme), and vanilla JavaScript — no framework, no bundler.
- Google Fonts (Space Grotesk · Inter · JetBrains Mono) and Font Awesome icons, loaded non-render-blocking.
- Responsive images: hero served as AVIF/WebP/JPG via `<picture>`; heavy dashboard/certificate screenshots served as WebP with PNG fallback.
- SEO: canonical URL, Open Graph + Twitter cards, JSON-LD `ProfilePage`/`Person`, `robots.txt`, and `sitemap.xml`.
- Accessibility: visible keyboard focus, accessible modal dialogs (lightbox + mobile drawer) with focus management, reduced-motion support, and labelled landmarks.

## Structure

```
index.html          # the entire site (markup, styles, script)
site.webmanifest    # PWA manifest
robots.txt          # crawler directives
sitemap.xml         # sitemap
photos/             # portrait, project & certificate images (+ optimized variants)
```

## Develop

It's a static site — just open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Served via GitHub Pages from the `main` branch.
