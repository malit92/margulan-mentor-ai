# Margulan Personal Mentor AI

[![Live](https://img.shields.io/badge/live-margulan--knowledge--platform.vercel.app-C8A368?style=flat-square)](https://margulan-knowledge-platform.vercel.app)
[![Deployed on Vercel](https://img.shields.io/badge/deployed%20on-Vercel-0E0E0F?style=flat-square&logo=vercel&logoColor=white)](https://vercel.com/ildar-mukhametzyanovs-projects/margulan-knowledge-platform)
[![Lighthouse](https://img.shields.io/badge/lighthouse-95%2B-brightgreen?style=flat-square)](https://pagespeed.web.dev/analysis?url=https%3A%2F%2Fmargulan-knowledge-platform.vercel.app)
[![A11y](https://img.shields.io/badge/a11y-WCAG%20AA-brightgreen?style=flat-square)](https://margulan-knowledge-platform.vercel.app)
[![Stack](https://img.shields.io/badge/stack-vanilla-F2EFEA?style=flat-square)](#stack)

> ## 🌐 [margulan-knowledge-platform.vercel.app](https://margulan-knowledge-platform.vercel.app)

Premium digital knowledge platform built on the structured philosophy of Margulan Seisembai — mission, energy, kaizen, awareness, leadership, and personal effectiveness.

> Editorial system, not SaaS landing.
> Cinema for thinking, not infotainment.

---

## Screenshot

<!-- To enable: add a 1600×1000 PNG/JPG at screenshots/hero.png (capture from the live URL on a desktop browser, dark theme), then uncomment the line below. -->
<!-- ![Margulan Personal Mentor AI — hero](screenshots/hero.png) -->

📸 _Coming — capture pending. Drop the file at `screenshots/hero.png` and uncomment the image reference above._

---

## Stack

- **Vanilla** HTML / CSS / JavaScript — single file, no build step
- **Fraunces** (variable serif) + **Inter** (variable sans) — self-restrained pair via Google Fonts (subset)
- **Mobile-first**, dark by default, brass-only accent
- **Editorial chapter-marks**, calm motion, AI-product feel
- **Static**: deployable to any CDN/edge in under a minute

## Performance

- Single ~100 KB HTML file (CSS + JS inline)
- 1 external request (subset Google Fonts CSS)
- `IntersectionObserver` for reveal animations — no scroll-listener cost
- `requestAnimationFrame` throttling for scroll handlers
- `prefers-reduced-motion` respected on every keyframe and transition
- `inert` attribute for proper modal isolation (mobile menu)

## Local

```bash
# Just open the file:
start index.html             # Windows
open index.html              # macOS

# Or serve with any static server:
python -m http.server 8000
# → http://localhost:8000
```

No dependencies. No build. One HTML file = production.

## Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fmalit92%2Fmargulan-mentor-ai)

### Via Vercel CLI

```bash
npm i -g vercel
vercel login
vercel           # preview
vercel --prod    # production
```

Vercel-specific config (security headers + cache control) lives in [vercel.json](vercel.json).

### Other hosts

Cloudflare Pages · Netlify · GitHub Pages · S3 + CloudFront — all work without modification. The `vercel.json` headers can be translated to a `_headers` file (Cloudflare/Netlify) or a CloudFront response policy.

## Project DNA

See [CLAUDE.md](CLAUDE.md) — full design system, architecture, coding standards, content rules, and continuation protocol for future contributors.

Highlights:
- **Design tokens** — full color palette, type scale, spacing system, motion language
- **Component patterns** — section template, expandable theme, pull-quote, dialogue, sticky-bar
- **Coding standards** — BEM-light naming, semantic HTML, vanilla JS in IIFE, `inert`/`aria` discipline
- **Future development rules** — what to extend, what never to change, what NOT to add

## Content sources

All quotations on the site are direct from publicly available transcripts of Margulan Seisembai's talks and interviews. Each quote carries attribution to the source talk. Platform copy (hero, section titles, CTAs) is clearly distinguishable from quoted material — no fake attribution.

## Disclaimer

The Personal Mentor AI shown on the site is a **curated demonstration**. It is a simulation built on publicly available material — not the real person. Live AI integration lives in a separate project.

---

© 2026 Margulan Personal Mentor AI · Static site
