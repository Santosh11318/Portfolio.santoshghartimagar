# Santosh Gharti Magar — AI Website Developer Portfolio

A production-ready, single-page business portfolio built with **pure HTML5, CSS3 and vanilla JavaScript** (no frameworks, no build step).

## Files

| File | Purpose |
|---|---|
| `index.html` | All page markup, SEO meta tags, JSON-LD schema |
| `style.css` | Full styling — glassmorphism, gradients, dark/light mode, animations, responsive layout |
| `script.js` | Interactivity — theme toggle, mobile nav, scroll reveal, counters, hero animation, accordion, testimonial slider, WhatsApp form |
| `robots.txt` | Search engine crawl rules |
| `sitemap.xml` | Sitemap for search engines |
| `assets/logo.png` | Your SGM Digital Marketing logo, background removed (full icon + wordmark) |
| `assets/logo-icon.png` | Cropped icon-only mark, used in navbar, favicon, footer and the loading screen |
| `assets/profile.jpg` | Your headshot, used in the About section |
| `README.md` | This file |

**Keep the `assets` folder next to `index.html`** — the site links to images at relative paths like `assets/logo-icon.png`, so the folder structure must stay intact when you upload/host it.

## Before you deploy — 3 things to update

1. **Domain** — replace every instance of `https://santoshghartimagar.com/` in `index.html`, `robots.txt` and `sitemap.xml` with your real domain once you buy/host one.
2. **OG image** — `og:image` / `twitter:image` point to `/assets/og-cover.jpg`, which doesn't exist yet. Add a 1200×630px cover image at that path (a screenshot of your hero section works well).
3. **Testimonials** — the four testimonials are realistic placeholders written around your actual project categories (salon, restaurant, clinic, business). Swap in real client quotes as you collect them.

## About the logo/photo and the Behance reference

- Your **SGM Digital Marketing logo** (gray background) had its background removed and was cropped into a clean icon mark — now used site-wide in the navbar, favicon, footer and loading screen.
- Your **headshot photo** now appears in the About section profile card.
- The third uploaded image (the office/monitor mockup with the logo and your photo composited in) was a moodboard-style render, not a usable web asset as-is, so it wasn't inserted directly — but its colour cues (dark charcoal + red/gold accents) are reflected in the icon and photo treatment.
- The Behance link you shared couldn't be opened directly (Behance blocks automated access), so the design wasn't copied pixel-for-pixel from it. The site instead follows the same general direction that link's title suggests — a modern, dark, glass-panel personal developer portfolio — combined with the glassmorphism/gradient brief from your original request.

## How the WhatsApp integrations work

- **Nav / hero / floating buttons**: direct `wa.me` links with a pre-filled greeting.
- **Contact form**: pure client-side JavaScript — on submit, it reads all form fields, builds a formatted message, and opens `https://wa.me/918799747981?text=...`. Nothing is stored or sent to a server.

## Hosting options

- **GitHub Pages** (free): push these files to a repo, enable Pages in repo settings, done.
- **Google Drive hosting** (as offered in your Services section): works for simple static hosting via drive-to-web tools, though GitHub Pages or Netlify/Vercel will give a cleaner, faster, custom-domain-ready result.
- **Netlify / Vercel** (free tier): drag-and-drop this folder for instant deployment with a free subdomain.

## Performance & SEO checklist already included

- Semantic HTML5 structure, ARIA labels, visible focus states, `prefers-reduced-motion` support
- Meta title/description/keywords, canonical URL, Open Graph + Twitter Card tags
- JSON-LD: `Person`, `LocalBusiness`, `WebSite`, `BreadcrumbList`
- `robots.txt` + `sitemap.xml`
- Lazy-loaded portfolio iframes, minimal external requests (only Google Fonts), no render-blocking scripts
- Mobile-first responsive design (desktop, laptop, tablet, mobile breakpoints)

## Notes for future edits

- All **Services**, **Portfolio**, **Why Choose Me**, **Testimonials** and **FAQ** content is data-driven from arrays at the top of `script.js` (`SERVICES`, `PROJECTS`, `WHY`, `TESTIMONIALS`, `FAQS`) — edit the arrays, not the HTML, to add or change entries.
- Dark mode is the default; the theme toggle remembers the visitor's choice via `localStorage`.
