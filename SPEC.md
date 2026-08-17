# Portfolio Website — Build Spec for Antigravity CLI

## 1. Project overview

Build a single-page personal portfolio website for **Saurav Dhungana**, an ML/AI Engineer based in Kathmandu, Nepal. The site should feel like an editorial magazine profile, not a generic SaaS/dev-template dark-mode site. Static site only — no backend, no database.

**Tech stack:** Plain HTML/CSS/JS (no framework needed) OR Next.js if you want it more maintainable long-term — either works. Deploy target: Vercel or GitHub Pages.

## 2. Design direction (do NOT default to generic AI-portfolio look)

Avoid the three clichés: (1) cream background + terracotta accent, (2) near-black + acid-green/neon accent, (3) broadsheet hairline-rule newspaper grid. Instead, use this specific direction:

**Concept:** Editorial magazine profile piece — like a print feature on a young engineer, built around his own black-and-white studio portraits.

**Color tokens:**
- `--bg`: `#0E0D0C` (warm near-black, not pure black)
- `--surface`: `#171513` (card/section backgrounds)
- `--text`: `#F2EEE6` (warm off-white, not pure white)
- `--text-muted`: `#948C7E` (secondary text, captions)
- `--accent`: `#C9A227` (muted brass/gold — used sparingly: links, small labels, one hover state)
- `--hairline`: `#2A2724` (dividers, borders)

**Typography:**
- Display/headline face: **Fraunces** (serif, editorial) — name, section titles, pull quotes
- Body face: **Inter** — paragraph text, nav
- Utility/mono face: **JetBrains Mono** — small labels, tech-stack tags, eyebrow text

Load fonts via Google Fonts.

**Layout concept:**
- Hero: large duotone-treated photo on one side, name in large Fraunces serif + role + short intro on the other. Subtle grain overlay on the photo. This is the signature visual moment.
- Sections separated by thin hairline dividers, generous vertical whitespace.
- Projects: real space per project, title in serif, one-line description, tech stack as mono pill tags, link out to GitHub/live demo.
- Skills: simple tag/pill cluster, mono font.
- Contact/footer: minimal — email, LinkedIn, GitHub, location, resume button (placeholder link fine for now).

**Motion:** Restrained. Subtle fade/slide-up on scroll per section. Respect `prefers-reduced-motion`.

**Quality bar:** Fully responsive to mobile, visible keyboard focus states, good text contrast.

## 3. Content

### Hero
- Eyebrow: `ML / AI ENGINEER`
- Name: `Saurav Dhungana`
- Intro (first person): "I build applied ML systems — RAG pipelines, embedding search, and full-stack AI products — while preparing for graduate study in AI/ML in Germany."
- Location: `Kathmandu, Nepal`

### About
2–3 sentences: BCA graduate from Nepal, hands-on builder who ships real projects, background also includes content/copywriting work, currently building toward ML/AI roles and a Master's in Germany.

### Projects (4, in order)

1. **GermanMatch AI** — SaaS platform helping international students find English-taught Master's programs at German public universities. Tech: FastAPI, pgvector, BAAI/bge-small-en-v1.5 embeddings, Gemini API (RAG), Playwright/BeautifulSoup. Give this the most visual weight.
2. **Second Brain Bot v2** — Personal knowledge-management RAG assistant. Tech: FastAPI, BAAI embeddings, Gemini API, SQLite with vector search.
3. **Ludo App** — Mobile Ludo game built for the Play Store. Tech: React Native, Expo.
4. **AI-Powered Health Risk Dashboard** — Final year BCA project, dashboard combining ML models for health risk indicators. Tech: Python/ML, Colab-trained models.

Leave `[GITHUB LINK]` and optional `[LIVE DEMO LINK]` placeholders for each.

### Skills
- **ML/AI:** Python, RAG pipelines, embeddings, vector search, Gemini API, scikit-learn
- **Backend:** FastAPI, SQLite, PostgreSQL/pgvector
- **Frontend/Mobile:** React Native, Expo, HTML/CSS/JS
- **Tools:** Playwright, BeautifulSoup, Git, Linux

### Contact / Footer
- Email: `sauravdhungana.official@gmail.com`
- LinkedIn: `https://www.linkedin.com/in/sauravdhungana12`
- GitHub: `https://github.com/sauravdhungana1`
- Location: Kathmandu, Nepal
- Resume button: placeholder link (`#`) for now

## 4. Photos

Two B&W studio portraits are already saved at `assets/hero.jpg` and `assets/secondary.jpg`. Use:
- `assets/hero.jpg` (seated, sunglasses, hands clasped, watch visible) as the main hero image
- `assets/secondary.jpg` (leaning on chair, hand in hair) as a secondary image in the About section or as a smaller accent elsewhere

Apply a subtle duotone treatment (black + brass accent at low opacity), or leave true B&W with a thin brass-colored border accent — pick whichever reads better.

## 5. Structure checklist

1. Hero (photo + name + intro + location)
2. About (short bio)
3. Projects (4 featured, generous spacing)
4. Skills (tag clusters)
5. Contact/Footer
6. Responsive breakpoints: mobile (<640px), tablet (640–1024px), desktop
7. Scroll-reveal animation per section (respect reduced-motion)
8. Deploy-ready: clean file structure, README with Vercel/GitHub Pages deploy instructions
