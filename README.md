# MetricTether Website

> A sleek, high-conversion static showcase for AI-agentic software products.

**Domain:** `metrictether.com`
**Tech Stack:** Astro 6 + Tailwind CSS v4 + TypeScript
**Deployment:** Cloudflare Pages — Build command: `npm run build`, Publish directory: `dist/client/`, Node 22

## Products Showcased

1. **Churn Analytics** — An autonomous AI email interviewer for SaaS subscription businesses.
2. **FreelancerCashFlow** — A comprehensive AI-powered financial operating system for freelancers and agencies.
3. **Custom AI Agents Sandbox** — Tailor-built micro-agents for specialized business operations.

## Development

All commands run from the project root:

| Command | Action |
| :------ | :----- |
| `npm install` | Installs dependencies |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `npm run build` | Builds production site to `./dist/` |
| `npm run preview` | Previews the build locally |

## Project Structure

```text
/
├── public/
│   ├── favicon.svg
│   ├── favicon.ico
│   ├── og-image.svg
│   ├── robots.txt
│   └── sitemap.xml
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── Products.astro
│   │   ├── HowItWorks.astro
│   │   ├── Waitlist.astro
│   │   ├── About.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── index.astro
│   │   └── 404.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── tailwind.config.js
└── package.json
```

## Design System

- **Primary Background:** `#0B0F17` (Deep Space Navy)
- **Accent Colors:** Cyan (`#38BDF8`), Emerald (`#10B981`), Crimson (`#F43F5E`)
- **Fonts:** Space Grotesk (headings), Inter (body), JetBrains Mono (code)
- **Form Integration:** Formspree
- **Analytics:** Plausible.io (privacy-focused)
# metritether-website
# metritether-website
