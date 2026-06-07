# Project 1 — Static Webpage Design
### DecodeLabs Frontend Development · Batch 2026

A fully semantic, accessible, and W3C-valid personal portfolio page built with pure HTML5 and CSS3. No JavaScript. No frameworks. Just structural mastery.

---

## 🔗 Quick Links

| | |
|-|-|
| **Live Page** | `P1.html` |
| **Stylesheet** | `P1.css` |
| **Author** | Danish Saeed |
| **Program** | DecodeLabs Batch 2026 |

---

## 🎯 Project Goal

Demonstrate that great frontend work starts before a single line of CSS is written. This project focuses on Information Architecture, semantic HTML structure, and a clean external CSS system — the foundation every other skill is built on.

---

## 📄 Page Sections

| Section | Element | Purpose |
|---------|---------|---------|
| Header | `<header>` | Fixed nav with logo + primary navigation |
| Hero | `<section>` | H1, eyebrow text, CTA button, hero image, scrolling ticker |
| About | `<section>` | Two-column layout, profile photo, quick-facts list |
| Skills | `<section>` | 3×2 grid of skill cards |
| Work | `<section>` | Asymmetric portfolio grid (1 large + 2 small cards) |
| Contact | `<section>` | Centered CTA with mailto link |
| Footer | `<footer>` | Copyright + footer nav |

---

## 🛠️ Techniques Used

### HTML5
- Semantic landmarks — `<header>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<figcaption>`, `<footer>`
- Single `<h1>` per page (Page Topic / Zero Point principle)
- Logical heading hierarchy — `h1 → h2 → h3`
- ARIA attributes — `aria-label`, `aria-labelledby`, `aria-hidden`
- `alt` text on every `<img>`; `aria-hidden="true"` on decorative elements
- `role="contentinfo"` on footer for screen reader landmark

### CSS Architecture
- **External stylesheet only** — zero inline styles, zero `<style>` blocks
- **BEM methodology** — `.block__element--modifier` naming throughout
- **DRY principle** — shared `.container`, `.btn`, `.section-label` utilities reused across sections
- **CSS custom properties** — full design token system in `:root`
- **No IDs used for styling** — classes only

### Layout
- CSS Grid — page-level two-column layouts (hero, about, work grid)
- Flexbox — navigation, fact list, footer, button groups
- Asymmetric work grid: `grid-column: 1 / -1` for featured card spanning full width

### Typography
- Google Fonts: **Fraunces** (display/headings) + **DM Sans** (body)
- `clamp()` for fluid heading sizes
- Controlled line-height, letter-spacing, and font-weight per context

### Animation
- Scrolling ticker — `@keyframes ticker-scroll` with `translateX`
- "Available" badge pulse — `@keyframes pulse-dot`
- Hover transitions — `transform: translateY(-2px)` on cards and buttons

### Responsive
- Breakpoint at `900px` — single-column hero, about, and work grid
- Breakpoint at `600px` — single-column skills, nav collapsed to CTA only

---

## 🎨 Design Tokens

| Token | Value |
|-------|-------|
| Background | `#0f0e0e` |
| Surface | `#1a1918` |
| Surface Alt | `#222120` |
| Accent (amber) | `#e8c547` |
| Text | `#f0ede8` |
| Muted Text | `#8a8480` |
| Border | `#2e2c2b` |
| Display Font | Fraunces |
| Body Font | DM Sans |

---

## ✅ Quality Checklist

- [x] W3C HTML Validator — zero errors
- [x] Single `<h1>` per page
- [x] External CSS only — no inline styles
- [x] BEM naming — consistent throughout
- [x] DRY CSS — shared utilities, no repetition
- [x] `alt` text on every image
- [x] ARIA labels on all nav and landmark elements
- [x] 4.5:1 minimum contrast ratio (WCAG AA)
- [x] Keyboard navigable
- [x] `aria-hidden` on all decorative/presentational elements
- [x] Smooth scroll via `scroll-behavior: smooth`
- [x] `overflow-x: hidden` — no horizontal scroll on any viewport

---

## 👤 Author

**Danish Saeed** — DecodeLabs Frontend Development Intern · Batch 2026
📧 [daanishsaeed593@gmail.com](mailto:daanishsaeed593@gmail.com)
🐙 [github.com/DanishCoderX](https://github.com/DanishCoderX)
