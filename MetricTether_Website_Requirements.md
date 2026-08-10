# MetricTether.com — Static Website Architecture & Design Requirement Document

**Version:** 1.1  •  **Status:** Final Draft / Implementation Ready
**Domain:** `metrictether.com`
**Vision:** A sleek, high-conversion static showcase for AI-agentic software products, financial intelligence tools, and smart customer analytics.

---

## 1. Executive Summary & Brand Positioning

### Brand Identity
* **Name:** MetricTether
* **Tagline:** *Intelligent Software & Agentic Workflows for Modern Businesses*
* **Core Value Proposition:** MetricTether builds pinpoint, AI-agentic software tools that automate complex workflows—from predicting and interviewing churned users to stabilizing freelancer cash flows. We "tether" deep analytical metrics to proactive, autonomous action.

### Product Portfolio
MetricTether develops and maintains **two distinct software products**, each solving a specific business-critical problem:

| Product | Target Audience | Core Problem |
| :--- | :--- | :--- |
| **Churn Analytics** | SaaS Founders, Product Managers, Subscription Businesses | Generic exit surveys yield shallow insights; manual offboarding churn interviews are too time-consuming. |
| **FreelancerCashFlow** | Freelancers, Agencies, Solopreneurs | Unstable income from late payments, no cash flow forecasting, and manual financial tracking. [App: cashflow.metrictether.com] |

> **Important:** These are independent products. Churn Analytics does **not** power FreelancerCashFlow and vice versa. They share a common agentic AI engine but solve entirely different operational bottlenecks.

### Target Audience (Combined)
1. **SaaS Founders & Product Managers** — seeking automated churn intelligence.
2. **Freelancers, Agencies & Solopreneurs** — needing predictability in cash flow, invoice tracking, and revenue forecasting.
3. **Tech-Forward SMBs & Enterprises** — seeking plug-and-play AI agents to optimize niche business bottlenecks.

---

## 2. Visual Aesthetic & UI/UX Guidelines

### Design System & Color Palette
* **Theme:** Clean Dark Mode base with high-contrast light accents.
* **Primary Background:** `#0B0F17` (Deep Space Navy/Charcoal)
* **Surface Layers:** `#121826` (Card backgrounds), `#1E293B` (Secondary surfaces)
* **Border/Dividers:** `#334155` (Slate-700), with glow variants for interactive states
* **Text:**
  * Headings: `#F1F5F9` (Slate-50)
  * Body: `#94A3B8` (Slate-400)
  * Muted captions: `#64748B` (Slate-500)
* **Accent Colors:**
  * **Agentic Blue / Cyan (`#38BDF8` / `#6366F1`):** Represents AI intelligence, precision, and telemetry.
  * **Emerald Green (`#10B981`):** Represents positive cash flow, retention, and growth metrics.
  * **Warning Crimson (`#F43F5E`):** Soft highlight for churn and financial leakages.
* **Typography:**
  * **Headings:** Space Grotesk (Modern, clean sans-serif, slightly futuristic).
  * **Body:** Inter (Optimized for readability across device screens).
  * **Code / Metrics Display:** JetBrains Mono (Monospaced for technical credibility).

### UI & UX Micro-Interactions
* **Glow Cards & Glassmorphism:** Subtle dark-mode card overlays with soft neon border glows on hover.
* **Animated Gradients:** Faint animated gradient background behind hero headline (cyan-indigo pulse).
* **Interactive Tool Previews:**
  * Churn Analytics: Mock interactive email exchange widget showing an AI agent responding to a cancelling user.
  * FreelancerCashFlow: Live financial dashboard mockup with cash flow projection graph.
* **Agentic Decision Flow Diagram:** SVG-based animated network diagram showing the 3-step agentic loop.
* **Fast & Lightweight:** Static site with minimal JS for lightning-fast loads.

### Responsiveness
* Mobile-first: 1-col (320px+) → 2-col (768px+) → 3-col (1024px+).
* Touch-friendly targets (44px min).
* Collapsible mobile nav menu.

### Accessibility
* WCAG AA compliance (4.5:1 contrast minimum).
* Focus-visible rings on interactive elements.
* Semantic HTML5 landmarks.
* Alt text on all images and decorative elements.

---

## 3. Recommended Tech Stack (Static Web)

| Layer | Recommended Choice | Rationale |
| :--- | :--- | :--- |
| **Framework** | **Astro** | Unmatched performance, zero-JS default, seamless content management. |
| **Styling** | **Tailwind CSS + Lucide Icons** | Utility-first styling for fast iterations and unified design. |
| **Language** | **TypeScript** | Type-safe development for future interactivity. |
| **Animation** | CSS animations + AOS library | Lightweight scroll-triggered animations. |
| **Forms & Lead Capture** | **Formspree** | Captures early-access signups without a custom backend. |
| **Analytics** | **Plausible.io** | Privacy-focused, lightweight analytics. |
| **Deployment** | **Vercel / Cloudflare Pages / Netlify** | Free global CDN with instant DNS. |

---

## 4. Key Website Sections & Page Architecture

Single-page layout with distinct sub-section anchors:

```
[ Header / Navigation ]
       │
       ├── 1. Hero Section (Hook + Value Prop + Primary CTA)
       ├── 2. Product Suite / Portfolio Grid (AI-Agentic Spotlight)
       │      ├── Churn Analytics (AI Email Interviewer)
       │      ├── FreelancerCashFlow (Full financial OS)
       │      └── Custom AI Agents Sandbox (Upcoming)
       ├── 3. How MetricTether Works (Interactive Agentic Workflow)
       ├── 4. Waitlist / Lead Generation
       ├── 5. About & Engineering Philosophy
       └── 6. Footer & Status
```

---

## 5. Detailed Breakdown of Required Page Elements

### 5.1. Navigation / Header
* **Logo Brandmark:** "MetricTether" wordmark with a geometric tether/network node icon (two connected nodes with a pulse line).
* **Nav Links:** `Products`, `How It Works`, `About`.
* **Primary CTA Button:** "Request Early Access" (glowing gradient button).
* **Mobile:** Hamburger → full-screen drawer menu.

### 5.2. Hero Section
* **Headline:**
  > *"Autonomous AI Agents That Guard Your Revenue & Stabilize Your Cash Flow."*
* **Sub-headline:**
  > *"MetricTether builds intelligent, agentic software tools that transform raw business telemetry into proactive automated workflows—from AI-driven churn interviews to dynamic cashflow forecasting."*
* **CTA Group:**
  * **Primary:** `[ Explore Our Products ↓ ]`
  * **Secondary:** `[ Join the Waitlist ]`
* **Hero Background:** Animated abstract network with pulsing nodes (cyan-indigo).
* **Tech Pill Badges:** `⚡ Powered by Agentic Workflows` · `🔒 Privacy First` · `📊 Real-Time Telemetry`

### 5.3. Flagship Products Suite (The Core Showcase)

Each product card highlights **Problem**, **AI-Agentic Solution**, and **Business Impact**.

#### Product 1: Churn Analytics — *Turn Exit Surveys into Conversational Insights*
* **Target:** SaaS founders, product managers at subscription businesses.
* **Problem:** Cancellation forms yield 1-word generic answers; manual offboarding interviews are too time-consuming.
* **Agentic Solution:** Autonomous AI interviewer agent triggers on customer cancellation. Sends personalised, context-aware email replies asking targeted follow-up questions based on the user's past product usage and stated reason for leaving.
* **Key Features:**
  * **Qualitative-to-Quantitative Mapping:** Translates natural email conversations into structured churn analytics dashboards.
  * **Autonomous Win-Back Offers:** Agent automatically negotiates custom retention discounts or pause options during the email thread.
  * **Root-Cause Classification:** Auto-categorises churn reasons (pricing, UX, feature gap, competitor, etc.) with confidence scores.
* **Visual:** Interactive email exchange widget mock.

#### Product 2: FreelancerCashFlow — *Predict, Protect, and Smooth Out Freelance Income Volatility*
* **Target:** Freelancers, agencies, solopreneurs.
* **Problem:** Unpredictable payment schedules, late invoices, and lumpy cash flow make financial planning impossible.
* **Agentic Solution:** Intelligent financial assistant that syncs with invoicing systems, analyses payment speeds of past clients, and models dynamic 30/60/90-day cash buffers.
* **Key Features:**
  * **Dashboard:** Health score with 3-phase unlock, net profit, goals, budgets, runway, aging, trends.
  * **Invoice Chasing:** 5-stage escalation with AI-generated content + late fee auto-calculation.
  * **Income Volatility Index (IVI):** Scores client payment risk before accepting retainer contracts.
  * **Agentic Expense Guard:** Suggests micro-reserves during high-income months to cover slow quarters.
  * **Double-Entry Accounting:** Chart of accounts, balance sheet, journal entries, P&L reports.
  * **Multi-Currency:** 35 currencies with live exchange rates (frankfurter.app).
  * **AI Payment Agent:** Ollama-powered invoice draft generation, recurring payment analysis, auto-follow-up.
  * **Bank Integration:** CSV import with auto-column detection + Plaid sync (configurable).
  * **Contracts & Proposals:** Full lifecycle from proposal to contract to invoice with status transitions.
  * **Client Portal:** Token-based invoice viewing + payment.
  * **Intake Forms:** Public project submission links.
  * **Team RBAC:** Admin/Editor/Viewer/Client roles.
  * **Security:** Rate limiting, CSRF, audit logging, AES-256-GCM encryption, MFA (TOTP).
* **Visual:** Cashflow projection graph (volatile vs. stabilized line chart).

#### Product 3: Custom AI Agents Sandbox — *Tailor-Built Micro-Agents for Specialized Operations*
* **Tagline:** *Build your own workflow-automation agents.*
* **Description:** Custom LLM-backed workflows designed for specific B2B operations—such as automated invoice auditing, lead scoring, vendor management, or any niche operational bottleneck.
* **Features:**
  * Scratch-built agents on demand.
  * Rapid deployment with plug-and-play integrations.
  * Fully auditable agent decision logs.
* **CTA:** `[ Pitch Us Your Workflow Bottleneck ]`

### 5.4. How "MetricTether Agentic Touch" Works (Explainer Section)
3-step visual infographic:
1. **Passive Observation (Ingestion)** — Connects to your stack, captures raw events (cancellations, bank feeds, payment delays, usage patterns).
2. **Autonomous Reasoning (Agentic Core)** — AI agent evaluates context, formulates strategy, executes outreach without human intervention.
3. **Tethered Action (Outcome)** — Insights logged, revenue recovered, cash flows rebalanced. Results feed back into the telemetry layer.

**Visual Element:** SVG animated decision-flow diagram with live telemetry status badge.

### 5.5. Waitlist / Lead Generation Section
* **Headline:** *"Be the First to Deploy MetricTether Agents."*
* **Subheadline:** *"Join a select group of early adopters getting priority access."*
* **Form Fields (Formspree):**
  * Name (required)
  * Email Address (required)
  * Product Interest Dropdown (required): `Churn Analytics`, `FreelancerCashFlow`, `Custom AI Agent Sandbox`
  * Textarea: *"What is your biggest operational or financial bottleneck?"*
* **Submit Button:** `[ Get Priority Access ]` (with loading + success states)

### 5.6. Footer
* **Copyright:** © 2026 MetricTether. All rights reserved.
* **Links:** `Privacy Policy`, `Terms of Service`, `GitHub`, `Twitter/X`, `LinkedIn`.
* **System Status Indicator:** `● All MetricTether Systems Operational` (green dot).

---

## 6. Actionable Implementation Checklist (Phase 1)

- [x] **Project initialized:** Astro CLI with TypeScript and Tailwind CSS.
- [ ] **Domain & DNS Setup:** Point `metrictether.com` nameservers to Vercel.
- [ ] **Design System Setup:** Tailwind configured with Navy/Cyan/Emerald color palette and typography.
- [ ] **Landing Page Construction:** Build responsive layout with Hero, Products, How-It-Works, Waitlist, About, Footer.
- [ ] **Form Integration:** Setup Formspree endpoint for waitlist capturing.
- [ ] **Analytics Setup:** Embed Plausible tracking.
- [ ] **SEO Meta Tags:** OpenGraph image, title tags, meta descriptions, sitemap.
- [ ] **Performance Check:** Lighthouse score ≥ 95 on mobile and desktop.

---

## 7. Next Steps for Iteration
1. **High-fidelity mockups:** Create visual designs for product cards.
2. **Deploy:** Push static build to `metrictether.com`.
3. **A/B test:** Hero headline and CTA variations.
4. **Add testimonials:** Early user quotes once available.
