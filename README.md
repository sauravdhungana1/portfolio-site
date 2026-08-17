# Saurav Dhungana — Personal Portfolio Website

An editorial magazine-style portfolio for **Saurav Dhungana**, ML / AI Engineer based in Kathmandu, Nepal.

Built with pure semantic HTML5, modern Vanilla CSS, and lightweight Vanilla JavaScript. Zero external frameworks or heavy dependencies.

---

## Visual & Design Philosophy

- **Concept**: Editorial magazine profile piece built around black-and-white studio portraits.
- **Palette**:
  - Background: Warm near-black (`#0E0D0C`)
  - Surface: Warm charcoal (`#171513`)
  - Typography Primary: Warm off-white (`#F2EEE6`)
  - Secondary/Muted: Warm clay (`#948C7E`)
  - Accent: Muted brass / gold (`#C9A227`)
  - Hairline borders: Refined dark border (`#2A2724`)
- **Typography**:
  - Display/Headlines: **Fraunces** (Editorial serif)
  - Body Text: **Inter** (High-legibility sans)
  - Code/Labels: **JetBrains Mono** (Technical monospace)

---

## File Structure

```text
portfolio-site/
├── assets/
│   ├── hero.jpg          # Primary studio portrait (Hero)
│   ├── hero.webp         # Modern WebP portrait asset
│   ├── secondary.jpg     # Secondary portrait (About section)
│   └── secondary.webp    # Modern WebP secondary asset
├── index.html            # Main semantic HTML5 document
├── style.css             # Vanilla CSS design system & layout
├── script.js             # Interactions (Scroll progress, reveal, clipboard)
├── SPEC.md               # Original project build specification
└── README.md             # Project documentation & deployment guide
```

---

## Local Development / Preview

You can preview the site with any local HTTP server:

```bash
# Using Python 3 built-in server
python3 -m http.server 8080

# Or using Node npx serve
npx -y serve .
```

Open [http://localhost:8080](http://localhost:8080) in your browser.

---

## Deployment Instructions

### 1. Deploying to Vercel

1. Push your code to a GitHub repository.
2. Go to [vercel.com](https://vercel.com) and click **"Add New Project"**.
3. Import your `portfolio-site` repository.
4. Framework Preset: Select **"Other"**.
5. Root Directory: `./` (or leave default).
6. Click **Deploy**. Vercel will instantly publish the static site with global CDN edge caching.

*Alternatively, deploy via Vercel CLI:*
```bash
npx vercel
```

### 2. Deploying to GitHub Pages

1. Push this folder to your GitHub repository (e.g. `sauravdhungana1/portfolio-site` or `sauravdhungana1.github.io`).
2. Go to the repository **Settings** → **Pages** (in the sidebar).
3. Under **Build and deployment**:
   - **Source**: Deploy from a branch
   - **Branch**: `main` (or `master`) / `/ (root)`
4. Click **Save**. Your site will be live at `https://<username>.github.io/<repo-name>/`.
