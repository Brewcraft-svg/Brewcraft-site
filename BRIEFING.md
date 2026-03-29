# BREWCRAFT — SITE BRIEFING FOR CLAUDE
# Read this first before making any changes.

---

## WHAT THIS IS

This is the complete website for **Brewcraft** — a UK-based branded packaging supplier
targeting independent cafés. The site is built in plain HTML/CSS/JS across 6 pages.
All files must stay in the same folder for navigation links to work.

---

## THE BUSINESS

**Business name:** Brewcraft (legal entity: Hertfordshire Trade Supplies)
**What they do:** Supply custom branded takeaway cups to independent cafés in the UK
**Positioning:** Branding-first packaging partner — not just a supplier
**Target customer:** Independent cafés, small chains (1–5 locations), boutique/lifestyle cafés
**USP:** End-to-end service (artwork, QR codes, supplier management, delivery) + personal service

**Key differentiators:**
- QR code integration (Google reviews, menus, loyalty, Instagram)
- Full artwork coordination included
- Personal service — real person on every order
- Repeat order discounts

---

## PRICING (current)

| Product         | First Order | Repeat Order |
|-----------------|-------------|--------------|
| 8oz double wall | £210/1k     | £175/1k      |
| 12oz double wall| £230/1k     | £195/1k      |

- Minimum order: 1,000 cups
- Setup fee: £35 per design (one-off, first order only)
- Bulk 5,000+: contact for pricing
- Lead time: 3–4 weeks (first), faster on repeats
- Delivery: included in price

---

## BRAND IDENTITY

**Colours:**
- Roast (primary):    #1E1C18  — deep espresso brown
- Cream (background): #F7F2E8  — off-white
- Cream dark:         #EDE6D6  — slightly darker cream for section backgrounds
- Seedling (accent):  #3B6D11  — deep craft green
- Warm (muted text):  #9A9588  — warm grey

**Typography:**
- Display/headings: Cormorant Garamond (serif, Google Fonts)
- Body/UI:          Syne (geometric sans, Google Fonts)

**Logo:** SVG inline in every page. Cup outline with 3 steam lines above in green.
Wordmark: "BREW" (bold) / "CRAFT" (regular weight) stacked.

**Tone of voice:** Confident, craft-aware, warm, direct. Never corporate.
**Tagline:** "Your brand. On every cup."

**Contact:**
- Email: hello@brewcraft.co.uk
- Instagram: @brewcraft
- Based: Hertfordshire, UK

---

## FILE STRUCTURE

```
brewcraft-site/
├── index.html          Homepage
├── why-us.html         Why Brewcraft page
├── how-it-works.html   Process / steps page
├── pricing.html        Pricing cards + volume table
├── faq.html            FAQ with category sidebar (dark bg)
└── contact.html        Enquiry form + what happens next
```

All pages share:
- Same nav (fixed top, links between all pages, "Get a quote" CTA in green)
- Same footer (logo + all links + copyright)
- Same colour variables
- Same font imports (Google Fonts)
- Active state on current page nav link

---

## PAGE SUMMARIES

### index.html — Homepage
- Hero: headline "Your cup is the first thing a customer holds. Make it count."
- Dark right panel with SVG cup illustration and 3 stats (1,000 MOQ / £210 / 3-4w)
- Quick links strip (4 boxes linking to each inner page)
- Brand strip (green bg) with 4 bullet points
- CTA band (dark bg)
- Footer

### why-us.html — Why Brewcraft
- 3 pillars: End to end / QR codes / Pricing loyalty
- 6-item included grid (2 cols)
- "Who is it for" section (dark bg, 3 cards)
- CTA band (green)

### how-it-works.html — Process
- 5 vertical steps with day/week timing tags (dark bg)
- Timing summary: 3 cards (3-4w / Faster / 24h)
- CTA band (green)

### pricing.html — Pricing
- 3 pricing cards: 8oz / 12oz (featured, dark) / Repeat orders
- Volume table (cream-dark bg)
- Setup fee explainer split section
- CTA band (green)

### faq.html — FAQ
- Dark background throughout
- Category sidebar nav: Ordering / Artwork / QR codes / Delivery / Payment
- 14 accordion questions across 5 groups
- CTA band (green)

### contact.html — Contact/Quote
- Split layout: left (info + what happens next) / right (form)
- Form fields: name, café name, email, phone, cup size, quantity, artwork status, message
- "What happens next" panel (dark)

---

## HOW TO MAKE CHANGES

### Text changes
Find the relevant file, locate the text, update it. Most content is in plain
`<p>`, `<h1>`, `<h2>`, `<h3>`, `<h4>` tags.

### Colour changes
Each file has a `:root {}` block near the top with CSS variables.
Change the hex value there and it updates site-wide within that file.
To change across ALL files, update each file's `:root {}` block.

### Pricing changes
Main location: pricing.html (cards + volume table)
Also appears in: index.html (hero stats), why-us.html (bullet points)

### Adding a new section
Add the HTML between existing sections, add matching CSS in the `<style>` block.
Follow the existing pattern: section tag → h2 → content.

### Adding a new page
1. Create new HTML file following the same structure
2. Add nav link to ALL 6 existing files
3. Add footer link to ALL 6 existing files

### Email address
Search for: hello@brewcraft.co.uk
Appears in: contact.html, footer of all pages (check each)

### Logo changes
The logo is an inline SVG repeated in the nav and footer of every page.
Search for `<svg viewBox="0 0 200 56"` to find each instance.

---

## SUPPLIER INFO (background, not on site)

Supplier: Elpack Packaging
- MOQ: 1,000 | Setup: £35/design
- Delivery: ~£9.95 (under 20kg) / ~£65 (pallet/5000+)
- Lead time: 3-4w first, shorter on repeats
- 12oz landed cost approx: £159.95 total (inc VAT + setup + delivery)

Margins: ~30% first order / ~35-40% repeat orders

---

## WHAT HASN'T BEEN BUILT YET

- Real form submission (currently a static button — needs Netlify Forms or similar)
- Real product photography (placeholder SVG cup illustration)
- Instagram feed embed
- Cookie/privacy policy page
- Google Analytics / tracking
- Domain + hosting (recommended: Netlify, free tier)

---

## PROMPT TO USE IN A NEW CHAT

Paste this at the start of any new Claude conversation:

"I'm working on the Brewcraft website — a branded cup supplier for independent cafés.
I have 6 HTML files: index.html, why-us.html, how-it-works.html, pricing.html,
faq.html, and contact.html. I'll upload the relevant file(s). Please read the
BRIEFING.md file first to understand the project, then make this change: [describe change]"

---
