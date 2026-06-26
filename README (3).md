# 🌐 Archana Vijayan — Personal Portfolio

> **Live:** [archanavijayan0112-spec.github.io](https://archanavijayan0112-spec.github.io) *(update once deployed)*

A fully responsive, single-file personal portfolio website built with pure HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, just code.

---

## ✨ Features

- **Typed hero animation** — cycles through role titles automatically
- **Scroll-reveal animations** — sections and cards fade in as you scroll
- **Animated skill bars** — trigger on scroll into view with smooth fill transitions
- **Project filter** — filter 12 projects by category (All / Featured / AI–ML / Web / Data / IoT)
- **Active nav highlighting** — nav link lights up for the current section
- **Responsive mobile nav** — hamburger menu with smooth open/close animation
- **Back-to-top button** — appears after scrolling 400px
- **Sticky blur navbar** — frosted-glass effect with scroll-aware border
- **Fully responsive** — tested from 320px mobile to 1440px+ desktop
- **No dependencies** — single `.html` file, Google Fonts loaded via CDN only

---

## 📁 Repository Structure

```
📦 portfolio
 ┣ 📄 index.html        ← Full portfolio (rename from archana_vijayan_portfolio.html)
 ┗ 📄 README.md         ← This file
```

> **Note:** Rename `archana_vijayan_portfolio.html` → `index.html` before deploying to GitHub Pages.

---

## 🚀 Deploy to GitHub Pages (Step-by-Step)

### Step 1 — Create the repository
1. Go to [github.com/new](https://github.com/new)
2. Name it exactly: `archanavijayan0112-spec.github.io`  
   *(must match your GitHub username exactly)*
3. Set it to **Public**
4. Click **Create repository**

### Step 2 — Upload files
1. Rename `archana_vijayan_portfolio.html` to `index.html`
2. In your new repo, click **Add file → Upload files**
3. Drag and drop both `index.html` and `README.md`
4. Commit with message: `Initial portfolio deploy`

### Step 3 — Enable GitHub Pages
1. Go to your repo → **Settings → Pages**
2. Under **Source**, select `Deploy from a branch`
3. Branch: `main` / `root` → click **Save**
4. Wait ~60 seconds, then visit: `https://archanavijayan0112-spec.github.io`

---

## 🛠️ Local Development

No build step needed. Just open the file in any browser:

```bash
# Option 1 — Direct open
open index.html

# Option 2 — Local server (recommended for live reload)
npx serve .
# or
python3 -m http.server 3000
```

---

## 🎨 Customisation Guide

All design tokens are in `:root` at the top of the `<style>` block:

```css
:root {
  --bg: #080810;           /* Page background */
  --accent: #7c6cfa;       /* Primary accent (purple) */
  --teal: #2dd4bf;         /* Secondary accent */
  --text: #eceaf5;         /* Primary text */
  --text-2: #9b97b2;       /* Secondary text */
  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'Inter', sans-serif;
}
```

### To update content

| Section | Where to look |
|---|---|
| Hero name / title | `<h1 class="hero-heading">` |
| Typed phrases | `const phrases = [...]` in `<script>` |
| Stats bar numbers | `.stat-num` spans inside `.stats-bar` |
| About text | `.about-text` paragraphs |
| Skill bars | `data-width="92"` attributes on `.skill-bar-fill` |
| Work experience | `.timeline-item` blocks |
| Projects | `.project-card` blocks in `#projects` |
| Certifications | `.cert-card` blocks in `#certifications` |
| Contact links | `.contact-link` anchors in `#contact` |

### To add a new project

```html
<div class="project-card" data-cat="web ml">   <!-- space-separated filter categories -->
  <div class="proj-badge badge-web">🌐 Web</div>
  <div class="proj-title">Your Project Title</div>
  <p class="proj-desc">Short description of what it does and why it matters.</p>
  <div class="proj-tech">
    <span class="ptag">Python</span>
    <span class="ptag">React</span>
  </div>
</div>
```

**Available filter categories:** `all` · `feat` · `ml` · `web` · `data` · `iot`

**Available badge classes:** `badge-feat` · `badge-ml` · `badge-web` · `badge-data` · `badge-sec` · `badge-mobile` · `badge-iot` · `badge-cloud` · `badge-ai`

---

## 🖥️ Sections Overview

| Section | Description |
|---|---|
| **Hero** | Name, typed role animation, CTA buttons, availability badge |
| **Stats Bar** | 5 key metrics — projects, certifications, internships, CGPA, automation gain |
| **About** | Bio paragraphs + 4 highlight cards |
| **Skills** | Animated progress bars (left) + categorised skill tags (right) |
| **Experience** | Timeline with two internships — Techmindz & Genzee Technologies |
| **Projects** | 12 filterable project cards with tech stacks |
| **Certifications** | 5 verified certifications with issuer and year |
| **Education** | B.Tech card with CGPA and key coursework areas |
| **Contact** | Links (email, phone, LinkedIn, GitHub) + availability card |

---

## 📱 Browser & Device Support

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Mobile Chrome/Safari | ✅ Full |

---

## 📄 License

This portfolio is personal work. You're welcome to use the code structure as inspiration or a template — just replace all content with your own.

---

## 👩‍💻 About

**Archana Vijayan** — CS Graduate, AI/ML Developer, Full-Stack Engineer  
📍 Palakkad, Kerala, India  
📧 archanavijayan0112@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/archana-vijayan-a67970322) · [GitHub](https://github.com/archanavijayan0112-spec)

---

*Built with ❤️ using HTML, CSS & vanilla JavaScript*
