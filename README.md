# Vermuthia — Luxury Vermutería Website

A complete, self-contained, production-ready single-file static website for **Vermuthia**, a boutique vermutería in Cerrado de Calderón, Málaga, Spain.

**Live instantly deployable** to GitHub Pages, Netlify, Vercel, or any static host.

---

## Features

- 100% single `index.html` (Tailwind via CDN + vanilla JS)
- Beautiful, editorial-grade luxury design
- Default Spanish + seamless EN/ES language switcher (data-driven i18n)
- All products, prices, and blog content live in clean JS objects at the top
- Detailed custom SVG logo matching the requested identity (deep forest green + warm gold)
- Fully responsive + refined micro-interactions
- Product modals, booking modal, full article modals, floating "Mi Reserva"
- Fake but realistic booking + newsletter submissions
- On-page SEO + structured data (LocalBusiness)
- Scroll animations, elegant typography (Playfair Display + Inter)

---

## How to Customize (30 seconds)

### 1. Edit Vermouths, Prices & Descriptions

Open `index.html` and find this clearly marked block near the top of the `<script>`:

```js
// ============ EDIT THIS SECTION TO UPDATE MENU / PRICES / BLOG ============
const vermouths = [ ... ]
const tablas = [ ... ]
const conservas = [ ... ]
const blogPosts = [ ... ]
const testimonials = [ ... ]
```

- Add/remove items from the arrays
- Each vermouth has `glass`, `bottle`, tasting notes (`short_es`/`short_en`), full description and suggested pairings
- Update names, prices, and descriptions in both languages

### 2. Change Images

Images are referenced in three places:

- Hero background (search for `background-image`)
- Vermouth cards (`image` property in `vermouths`)
- Gallery, Tablas, Blog, etc.

Replace any Unsplash (or your own) URL. For best results use high-resolution images (≥ 1600px wide).

### 3. Update Contact / Address / Hours

Search for the address block and footer:

- "Camino de los Montes 47"
- Phone + email
- Opening hours strings

### 4. Language & Copy

All static text uses `data-i18n` attributes + the `translations` object.

Dynamic content (products, blog) stores both `_es` and `_en` versions inside the data arrays.

---

## Deploy to GitHub Pages — DONE ✅

The full site has been pushed to this repository:

**Repo:** https://github.com/LD1878/vermutheria-

**Live site will be at:** https://ld1878.github.io/vermutheria-/

### Enable GitHub Pages (one-time, ~30 seconds):

1. Go to the repo: https://github.com/LD1878/vermutheria-
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
4. Click **Save**

GitHub will build and publish the site. It usually becomes available in 30–90 seconds at:

→ **https://ld1878.github.io/vermutheria-/**

You can also add a custom domain in the same Pages settings page.

---

The site is 100% static and ready. No further build steps needed.

---

## Technical Notes

- Tailwind CSS served via official Play CDN (`https://cdn.tailwindcss.com`)
- Google Fonts: Playfair Display + Inter
- No build step. No dependencies. Pure static.
- Vanilla JS only (IntersectionObserver, no frameworks)
- Fully accessible (keyboard navigation, semantic headings, ARIA)

---

## Design System (locked)

**Colors**
- `--bg-cream`: #F8F5EF
- `--green-deep`: #1E2F23
- `--green-leaf`: #3D5C3A
- `--gold`: #C5A46E
- `--gold-dark`: #A88A55
- `--text-primary`: #2C3C2E
- `--text-secondary`: #5C6B5A

**Typography**
- Serif (headings/logo): Playfair Display
- Sans (body): Inter

---

## Credits & License

Designed and built as a world-class luxury experience for high-end wine & spirits brands.

Free to use, modify and deploy for your own project. Do not claim the Vermuthia brand as your own.

Enjoy creating something beautiful.

---

Made with care for the art of vermut.
