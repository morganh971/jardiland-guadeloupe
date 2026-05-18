# Jardiland Guadeloupe — WordPress / Elementor Integration Guide

## Overview

This package contains the **complete website structure** for Jardiland Guadeloupe (garden center & pet store chain in Guadeloupe, French Caribbean): **30 static HTML pages** designed as the **reference for WordPress + Elementor Pro integration**.

The HTML files are fully functional, navigable, mobile-responsive, and reflect the final visual style. Your job is to recreate the structure inside WordPress, page by page, using Elementor Pro.

---

## Package Contents

```
jardiland-website/
├── INTEGRATION-GUIDE.md             ← This file (English)
├── MIDJOURNEY-PROMPTS.md            ← All Midjourney prompts for image generation (French)
├── index.html                       ← Homepage
├── blog.html                        ← Blog listing
│
├── article-arbres-fruitiers.html    ← Blog article 1
├── article-plantes-secheresse.html  ← Blog article 2
├── article-potager-creole.html      ← Blog article 3
├── conseils-plantes-medicinales.html ← Blog article 4 (long-form pillar)
│
├── pepiniere.html                   ← HUB Pépinière
├── pepiniere-plantes-exterieur.html
├── pepiniere-plantes-interieur.html
├── pepiniere-fruitiers.html
├── pepiniere-potager.html
│
├── animalerie.html                  ← HUB Animalerie
├── animalerie-chiens-chats.html
├── animalerie-rongeurs.html
├── animalerie-aquariophilie.html
│
├── outils.html                      ← HUB Outils & Entretien
├── outils-jardin.html
├── outils-engrais.html
├── outils-arrosage.html
│
├── plein-air.html                   ← HUB Plein Air & Déco
├── plein-air-mobilier.html
├── plein-air-barbecues.html
├── plein-air-piscines.html
│
├── catalogue.html                   ← Catalogue & promotions
│
├── magasins.html                    ← HUB Stores
├── magasin-baie-mahault.html        ← Store detail
├── magasin-les-abymes.html          ← Store detail
│
├── services.html                    ← HUB Services
├── services-livraison.html
├── services-financement.html        ← Includes #conseil anchor for "Conseil personnalisé"
│
├── assets/
│   ├── site.css                     ← Shared stylesheet (used by 24 of 30 pages)
│   └── header-footer-snippets.html  ← Reference markup for header/footer
│
├── fonts/
│   ├── Jardiland-Regular.otf
│   ├── Jardiland-Regular Italic.otf
│   ├── Jardiland-SemiBold.otf
│   ├── Jardiland-Bold.otf
│   ├── Jardiland-Heavy.otf
│   ├── Shelby-W05-Bold.otf
│   └── Shelby-W05-Bold.ttf
│
└── images/
    ├── logo-jardiland.svg
    └── ... (8 existing photos + 33 to be generated via Midjourney)
```

---

## Site Architecture (27-page SEO structure)

| URL | Page | Role |
|---|---|---|
| `/` | Homepage | Orientation, key sections |
| `/conseils/` | Blog hub | Editorial pillar |
| `/conseils/plantes-medicinales-creoles/` | Long-form article | High-potential local content |
| `/pepiniere/` | Hub | Plant offer overview |
| `/pepiniere/plantes-exterieur/` | Sub-page | Outdoor tropical plants |
| `/pepiniere/plantes-interieur/` | Sub-page | Indoor plants |
| `/pepiniere/fruitiers/` | Sub-page | Fruit trees |
| `/pepiniere/potager-creole/` | Sub-page | Vegetable garden |
| `/animalerie/` | Hub | Pet department |
| `/animalerie/chiens-chats/` | Sub-page | Dogs & cats |
| `/animalerie/rongeurs/` | Sub-page | Rodents |
| `/animalerie/aquariophilie/` | Sub-page | Aquariums |
| `/outils-entretien/` | Hub | Tools & care |
| `/outils-entretien/outillage-jardin/` | Sub-page | Garden tools |
| `/outils-entretien/engrais-terreaux-traitements/` | Sub-page | Fertilizers |
| `/outils-entretien/arrosage/` | Sub-page | Watering |
| `/plein-air-deco/` | Hub | Outdoor & decoration |
| `/plein-air-deco/mobilier-jardin/` | Sub-page | Garden furniture |
| `/plein-air-deco/barbecues-planchas/` | Sub-page | BBQ |
| `/plein-air-deco/piscines-kit-bassins/` | Sub-page | Pools |
| `/catalogue/` | Promotions | Catalogue PDF & offers |
| `/magasins/` | Hub | Store locations |
| `/magasins/baie-mahault/` | Store detail | |
| `/magasins/les-abymes/` | Store detail | |
| `/services/` | Hub | Services overview |
| `/services/livraison/` | Sub-page | Home delivery |
| `/services/financement-conseil/` | Sub-page | Financing & personal advice |

⚠️ **The HTML uses flat filenames** (e.g. `pepiniere-fruitiers.html`) for ease of preview. In WordPress, recreate the **nested URL structure** above using page parents (Pages > parent dropdown).

---

## Step 1: Install Custom Fonts

Before building anything, install the brand fonts in WordPress.

### Recommended: Elementor Pro Custom Fonts
1. Go to **Elementor > Custom Fonts**
2. Add font family **"Jardiland"** with these weights:
   - Regular (400) → `Jardiland-Regular.otf`
   - Regular Italic (400i) → `Jardiland-Regular Italic.otf`
   - SemiBold (600) → `Jardiland-SemiBold.otf`
   - Bold (700) → `Jardiland-Bold.otf`
   - Heavy (900) → `Jardiland-Heavy.otf`
3. Add font family **"Shelby"**:
   - Bold (700) → `Shelby-W05-Bold.ttf` (TTF preferred for browser compat)
4. **Body fallback**: Inter (Google Font, available natively)

---

## Step 2: Set Global Colors

In **Elementor > Site Settings > Global Colors**:

| Name | Hex | Usage |
|---|---|---|
| Primary (Orange) | `#E35205` | Buttons, CTAs, accents, hero badges |
| Primary Dark | `#c44600` | Hover states |
| Primary Light | `#ff6a1a` | Hero accent text, highlights |
| Green Dark | `#2a5a32` | Engagements section bg |
| Green Light | `#6aad6a` | Engagement icons, labels |
| Green Soft | `#e8f5e9` | Badge backgrounds |
| Dark | `#1a1a1a` | Body text, footer, reassurance bar |
| Dark Soft | `#2d2d2d` | Italic tip-box body |
| Gray | `#5a5a5a` | Body text |
| Gray Light | `#9a9a9a` | Subtle text |
| Off-white | `#faf9f7` | Section backgrounds |
| Cream | `#f3efe8` | Alt sections, tip-box bg |
| Gold | `#eec53a` | Star ratings |

---

## Step 3: Set Global Typography

In **Elementor > Site Settings > Global Fonts**:

| Role | Font | Weight | Size desktop |
|---|---|---|---|
| Primary (H1) | Jardiland | 900 | clamp(2.2rem, 5vw, 3.6rem) |
| Secondary (H2) | Jardiland | 900 | clamp(2rem, 4vw, 3rem) |
| H3 | Jardiland | 700 | 1.05–1.25rem |
| H4 | Jardiland | 700 | 1.05rem |
| Body | Inter | 400 | 1rem (16px) |
| Accent | Shelby | 700 | 2rem (used in `.cat-card-baseline` only) |

---

## Step 4: Page Templates — Recurring Patterns

The 30 pages reuse **a small set of patterns**. Build these once as **Elementor templates** and reuse them.

### Pattern A: Page Hero (used on all sub-pages)
- Section: full-width
- Background: image + dark gradient overlay (135deg, `rgba(26,26,26,0.65)` → `rgba(227,82,5,0.25)`)
- Min-height: 420px, padding 80px 24px
- Margin-top: 72px (to clear fixed header)
- Inside: badge pill (uppercase) → H1 (Jardiland 900, white) → subtitle (white, 90% opacity)

### Pattern B: Breadcrumb
- Light cream background (`#f3efe8`), padding 14px 24px
- Inline links: Accueil > Section > Page

### Pattern C: Hub category grid (`.cat-grid`)
- Grid: `repeat(auto-fit, minmax(280px, 1fr))`, gap 24px
- Each card: image with gradient overlay, tag pill, H3 (Jardiland 900), baseline (Shelby 2rem)
- Hover: overlay shifts to orange tint, arrow appears top-right
- **In Elementor**: use **Image Box** widget styled with custom CSS, or use a **Posts Grid** (Pro) if you want it dynamic

### Pattern D: Two-column section (`.two-col`)
- Grid: `1fr 1fr`, gap 60px, vertical center
- Left: image (border-radius 24px, aspect 4/5 or 4/3)
- Right: section-label → H2 → info-list (3 items with orange icon + title + paragraph)

### Pattern E: Highlight banner
- Solid `#E35205` background with decorative circles
- Centered: H2 (white) → paragraph → white pill button
- Padding 72px 24px

### Pattern F: Content block (long text pages)
- Max-width 800px, centered
- H2 spaced 48px top, 18px bottom
- H3 spaced 32px / 14px
- Bullet lists with custom orange dot bullets
- Numbered lists with Jardiland 900 orange numbers
- `.tip-box` callouts: cream bg, left border 4px orange, italic text

### Pattern G: CTA Section
- Gradient `#E35205 → #c44600` (135deg)
- Centered: H2 (white) → paragraph → button(s)
- Padding 90px 24px

### Pattern H: Header (mega-menu)
- Fixed position, white blurred background
- Logo + 8 nav items including 5 with hover-dropdowns:
  - Pépinière ▾ (5 sub-items)
  - Animalerie ▾ (4 sub-items)
  - Outils & Entretien ▾ (4 sub-items)
  - Plein Air & Déco ▾ (4 sub-items)
  - Conseils (single)
  - Catalogue (single)
  - Magasins ▾ (3 sub-items)
  - **Nos services** (CTA orange pill, single link)

⚠️ **In Elementor**: build the header via **Theme Builder**. Use the **Nav Menu widget** (Pro) and configure dropdown menus via WordPress > Appearance > Menus.

### Pattern I: Footer
- Dark `#1a1a1a` background
- 4 columns: logo + tagline + social, "Univers", "Jardiland", "Informations"
- Bottom: copyright + Katchak credit

⚠️ **In Elementor**: build the footer via **Theme Builder** > Footer.

---

## Step 5: Page-by-Page Content

The HTML files are **the source of truth** for content. For each page:

1. **Open the HTML file in a browser** to see the final visual
2. **View source** to copy text content (titles, paragraphs, bullet lists)
3. **Recreate the layout in Elementor** using the patterns above
4. **Plug in the same images** (filenames listed in `MIDJOURNEY-PROMPTS.md`)

The `assets/site.css` file contains all CSS classes used throughout the static site — it's a useful reference for spacing, colors, and component styles.

---

## Step 6: Images

See `MIDJOURNEY-PROMPTS.md` for all **33 image prompts** to generate. Each prompt:
- Specifies the exact target filename
- Specifies the recommended aspect ratio
- Provides a Midjourney v6 prompt with `--s 250` for visual consistency

**Workflow**:
1. Generate all images in Midjourney (33 total)
2. Upscale each in HD
3. Optimize via [Squoosh](https://squoosh.app/) — target 200-300 KB per JPG
4. Upload to WordPress media library with **the exact filenames** indicated

⚠️ **8 images already exist** in `images/` and should be kept as-is.

---

## Step 7: SEO Setup

For each page, configure (via Yoast or Rank Math):

- **Page title** (≤60 chars) — already in HTML `<title>` tag
- **Meta description** (~155 chars) — write based on H1 + intro paragraph
- **Canonical URL** — set to the WordPress URL
- **Open Graph image** — use the page's hero image
- **Schema markup** — `Organization` for homepage, `LocalBusiness` for store pages, `Article` for blog posts

### Critical local SEO fields
For both store pages, add **LocalBusiness** schema:

```json
{
  "@type": "GardenStore",
  "name": "Jardiland Baie-Mahault",
  "address": {
    "streetAddress": "Centre commercial Jardi-Village, Jabrun",
    "addressLocality": "Baie-Mahault",
    "postalCode": "97122",
    "addressCountry": "GP"
  },
  "telephone": "+590590606700",
  "openingHours": ["Mo-Sa 08:30-19:00", "Su 09:00-13:00"]
}
```

Same template for Les Abymes (97139, +590590300266).

---

## Step 8: Recommended WordPress Plugins

| Plugin | Purpose |
|---|---|
| Elementor Pro | Page builder (already required) |
| Yoast SEO or Rank Math | SEO meta + sitemaps |
| WP Rocket or LiteSpeed Cache | Performance |
| Smush or ShortPixel | Image optimization |
| WPForms or Elementor Forms | Newsletter form |
| Code Snippets | For custom CSS or PHP without editing theme |

---

## Step 9: Performance Checklist

- [ ] All Jardiland fonts uploaded with `font-display: swap`
- [ ] All images <300 KB, lazy-loaded (Elementor does this by default)
- [ ] Critical CSS inlined for above-the-fold (page hero)
- [ ] Mobile menu toggles correctly with dropdowns
- [ ] Page Speed Insights ≥85 mobile, ≥90 desktop
- [ ] Schema validated via [Schema Markup Validator](https://validator.schema.org/)

---

## Step 10: Going Live

Before launch:

- [ ] All 33 Midjourney images generated and uploaded
- [ ] All 27 pages built in Elementor
- [ ] Header + footer set as default in Theme Builder
- [ ] Permalinks structure: `/post-name/` (or custom by silo)
- [ ] All pages set with correct **page parent** to reflect URL hierarchy
- [ ] Newsletter form configured with provider (Mailchimp, Brevo, etc.)
- [ ] Google Analytics 4 + Google Search Console connected
- [ ] XML sitemap generated and submitted to GSC
- [ ] Old URLs (if any) 301-redirected to new ones

---

## Notes

- **All content is in French** — do not translate
- **No e-commerce** — site is purely informational/showcase
- The brand orange `#E35205` is the dominant accent color
- Shelby font is used **only** in `.cat-card-baseline` (italic handwriting style)
- The 4 blog articles + the medicinales pillar use long-form `.content-block` (max-width 800px, optimized for reading)
- Phone numbers throughout the site use `tel:` links for mobile click-to-call
- Both stores share the same opening hours: **Mon-Sat 8h30-19h, Sun 9h-13h**

## Contact

For any question on the design system, refer to `assets/site.css` (extensively commented) and the static HTML files which serve as the canonical visual reference.
