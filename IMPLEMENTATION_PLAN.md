# Codeinum Agency — Portfolio Website Implementation Plan

## Goal

Build a **high-converting, dark-mode agency portfolio** that positions you as a premium software & automation agency — optimized for Upwork, Fiverr, LinkedIn, and organic Google search to win freelancing clients **100× more effectively** than a generic profile.

---

## Tech Stack Decision

| Choice | Rationale |
|---|---|
| **Vite** (vanilla JS mode) | Blazing-fast dev server, zero-config, outputs optimized static assets |
| **Vanilla HTML / CSS / JS** | No framework bloat — ultra-fast load times impress clients & score perfect Core Web Vitals |
| **Google Fonts (Inter + JetBrains Mono)** | Modern, highly legible typography |
| **CSS custom properties + utility classes** | Full design-system control, dark-mode built-in |
| **Netlify / Vercel** (deploy later) | Free hosting with automatic SSL & global CDN |

> [!NOTE]
> No React/Next.js — a static portfolio doesn't need a SPA framework. This keeps the site under **50 KB** gzipped, loading in < 1 second, which itself demonstrates your performance expertise to potential clients.

---

## Freelancing 100× Strategy (Built Into the Site)

These principles will be **baked into every page**, not bolted on:

1. **Outcome-first copywriting** — Every headline leads with a business result, not a technology name
2. **Social proof density** — Testimonials, metrics, and logos appear on every page
3. **Friction-free contact** — CTA visible above the fold on every page; Calendly embed for instant booking
4. **Case-study depth** — Problem → Solution → Results format with quantified outcomes (the #1 thing clients scan for on Upwork)
5. **SEO & Open Graph** — Every page has unique title, description, and OG image so links shared on Upwork/Fiverr/LinkedIn look professional
6. **Speed as proof** — A portfolio that loads in < 1s says more than any "I build fast websites" claim
7. **Downloadable proposal template** — A CTA that offers a free project checklist in exchange for contact info (lead magnet)

---

## Phased Delivery — One Feature, One Commit

Each phase below maps to **one focused commit** pushed to GitHub.

---

### Phase 1 — Project Scaffolding & Design System  
**Commit message:** `feat: project scaffolding and design system`

#### Files
| File | Purpose |
|---|---|
| `index.html` | Entry point with SEO meta, OG tags, font links |
| `style.css` | Full design system — colors, typography, spacing, utilities, animations |
| `main.js` | Minimal JS (mobile nav toggle, smooth scroll) |
| `vite.config.js` | Vite config |
| `package.json` | Dependencies |
| `.gitignore` | Node modules, dist |
| `public/` | Favicon, OG image placeholder |

#### Design Tokens (CSS Custom Properties)
- **Background:** `#0a0a0f` (near-black) → `#12121a` (card surfaces)
- **Text:** `#e4e4e7` (body) / `#ffffff` (headings)
- **Accent Primary:** `#6366f1` (electric indigo)
- **Accent Secondary:** `#a855f7` (vibrant purple)
- **Accent Gradient:** `linear-gradient(135deg, #6366f1, #a855f7)`
- **Border:** `rgba(255,255,255,0.06)`
- **Glass effect:** `backdrop-filter: blur(16px); background: rgba(18,18,26,0.7)`

---

### Phase 2 — Homepage (Hero + Services Overview + Featured Work + Testimonials)
**Commit message:** `feat: homepage with hero, services, featured work, and testimonials`

#### Sections
1. **Hero** — Headline: *"Accelerating Business Growth Through Custom Software & Automation"*, subtext, animated gradient orb background, two CTAs ("Get a Quote" + "View Our Work")
2. **Trusted By** — Logo strip (placeholder logos with subtle animation)
3. **Services Overview** — 4 cards with hover-reveal tech icons (MERN, CMS, App Dev, Automation)
4. **Featured Work** — 3 project cards (one MERN, one CMS, one Automation) with image, title, tags, result metric
5. **Testimonials** — Carousel/grid of 3 client quotes with name, role, star rating
6. **CTA Banner** — "Let's Build Something Great" with contact button

---

### Phase 3 — Services Page
**Commit message:** `feat: services page with detailed offerings`

#### Content
- Hero banner with headline
- 4 detailed service sections (MERN Stack, CMS Integration, App Development, Automation)
- Each section: description, process steps, technology icons, a mini case-study snippet, CTA
- Interactive accordion or tab UI for technology deep-dives

---

### Phase 4 — Portfolio / Case Studies Page
**Commit message:** `feat: portfolio page with case study template`

#### Structure
- Filterable grid of project cards (filter by category)
- Individual case study layout following PRD structure:
  - Project Title & Client
  - Problem Statement
  - Solution
  - Technologies Used (with icons)
  - Key Features
  - Results & Impact (metric cards)
  - Visual Evidence (screenshot gallery + Loom video embed placeholder)

---

### Phase 5 — About Us Page
**Commit message:** `feat: about us page with team and values`

#### Content
- Agency story section
- Team member cards (photo, name, role, short bio, social links)
- Core values / differentiators (icon + text blocks)
- Timeline of milestones
- "Why Choose Us" comparison grid

---

### Phase 6 — Contact Page
**Commit message:** `feat: contact page with form and scheduling`

#### Content
- Contact form (Name, Email, Project Type dropdown, Budget Range, Message)
- Form submission via Formspree or similar (no backend needed)
- Calendly embed for instant consultation booking
- Direct email + social links
- FAQ accordion (common client questions)

---

### Phase 7 — Polish, Performance & Deployment
**Commit message:** `feat: final polish, animations, and performance optimization`

- Page transition animations
- Scroll-triggered reveal animations (Intersection Observer)
- Lazy-load images
- Generate OG images for each page
- Lighthouse audit → target 95+ on all metrics
- README with setup instructions
- Deployment to Netlify/Vercel

---

## User Review Required

> [!IMPORTANT]
> **Agency Name & Branding** — The PRD references "our agency" but doesn't specify a name. I'll use **"Codeinum"** based on the repo name `codeinum-portfolio`. Please confirm or provide the actual agency name.

> [!IMPORTANT]
> **Real Content vs Placeholder** — Should I use realistic placeholder content (fake project names, fictional client testimonials) for now, or do you have real projects/testimonials you'd like included? I'll start with high-quality placeholder content that you can swap later.

> [!IMPORTANT]
> **Calendly / Scheduling Tool** — Do you have a Calendly (or similar) link for the Contact page? I can add a placeholder embed that you swap later.

## Open Questions

1. **Color Preference** — The PRD suggests deep blues + accent colors. I've proposed **electric indigo (#6366f1) + vibrant purple (#a855f7)** on a near-black background. Does this palette appeal to you, or would you prefer a different accent (e.g., neon blue, teal, emerald)?

2. **Domain** — Do you have a custom domain, or will this live on a Netlify/Vercel subdomain for now?

3. **Multi-page vs Single-page** — The PRD describes separate pages. I'll build it as a **multi-page site** (separate HTML files) for better SEO. Is that okay, or would you prefer a single-page app with scroll sections?

---

## Verification Plan

### Automated
- `npm run build` — ensures Vite builds cleanly after each phase
- Lighthouse CI audit targeting 95+ scores
- HTML validation (W3C)

### Manual
- Browser testing (Chrome, Firefox, Safari) at desktop, tablet, mobile breakpoints
- Visual review of each page via `npm run dev`
- Link verification (all CTAs, nav links, social links work)

### Browser Testing
- After each phase, I'll run the dev server and visually verify the page in the browser tool
