# AGENTS.md — MetricTether Website

**Project:** MetricTether static showcase website
**Framework:** Astro 6.4.8
**Styling:** Tailwind CSS v4 + custom design system
**Status:** MVP complete

## Overview

Static website showcasing two AI-agentic software products:
1. **Churn Analytics** — Autonomous AI email interviewer for SaaS churn recovery
2. **FreelancerCashFlow** — Comprehensive financial OS for freelancers (reference: AGENTS.md in /home/desalegn/freelancer-cashflow/)

## Design System

- **Colors:** `#0B0F17` (navy), `#121826` (surface), `#38BDF8` (cyan), `#10B981` (emerald), `#F43F5E` (crimson)
- **Fonts:** Space Grotesk (headings), Inter (body), JetBrains Mono (code)
- **Tailwind v4:** Fonts and colors configured via `@theme` directive in `src/styles/global.css`
- **Component classes:** Use utility classes directly in Astro components (no `@apply` in CSS)

## Build Commands

```sh
npm run dev      # Local dev at localhost:4321
npm run build    # Production build to dist/
npm run preview  # Preview production build
```

## Conventions

- Use inline SVGs instead of icon libraries (keeps bundle tiny)
- All pages import `../styles/global.css` directly
- Single-page layout with anchor navigation (`#products`, `#how-it-works`, etc.)
- Contact: `info@metrictether.com`, `+4915755995080`
- Formspree endpoint for waitlist: configured in Waitlist.astro
- Plausible analytics: `data-domain="metrictether.com"`
- Hosting: Cloudflare Pages (build: `npm run build`, publish: `dist/client/`, Node: 22 from `.nvmrc`)
- Cloudflare adapter: `@astrojs/cloudflare` pre-installed (avoids auto-detection install failures)

## File Structure

```
src/
  components/     # All Astro components for each section
  layouts/        # Layout templates
  pages/          # Route pages (index, 404)
  styles/         # Global CSS + Tailwind config
public/           # Static assets (favicon, og-image, robots, sitemap)
```
