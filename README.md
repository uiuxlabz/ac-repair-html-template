# AERION — Climate Control & HVAC Service Website Template

A premium, framework-free HTML/CSS/vanilla-JS template for air conditioning, heating, and HVAC service companies. Built bespoke from the subject — not a recolored scaffold.

**Live preview:** `index.html` (open in browser)
**Stack:** HTML5 · CSS3 (custom properties, Grid, Flex) · Vanilla JS (no build step)
**Fonts:** Barlow Condensed (display) · Inter (body) · JetBrains Mono (labels/data) — all via Google Fonts
**License:** MIT — use commercially, modify freely.

---

## Pages

| Page | Description | Link |
|------|-------------|------|
| **Home** | Live status bar, industrial hero panel with thermostat gauge, readout stats (4 cells), 6 diagnostic service modules, feature split, emergency band, 3-tier pricing, testimonials, FAQ accordion, CTA | [index.html](index.html) |
| **About** | Page head, readout stats, company story split, 4 operating principles, team photo grid (4 cards), CTA | [about.html](about.html) |
| **Services** | Page head, 5 detailed service modules (AC repair, heating, installation, maintenance, air quality) in alternating image/text splits, emergency band, service area coverage grid, CTA | [service.html](service.html) |
| **Contact** | Contact form with service type + equipment + urgency selects, inline validation, info cards (emergency line, email, office, licensing) | [contact.html](contact.html) |

---

## Design Distinction

**This template was authored fresh for an HVAC/climate-control subject and diverges from every sibling template on all 6 divergence axes:**

| Axis | AERION (this template) | Sibling templates (MERIDIAN, SOURA, KORVA, VOSSEN, OLIVO) |
|------|----------------------|------------------------------------------------------------|
| **Hero composition** | Industrial control panel: dark metal background, thermostat dial gauge (conic-gradient + needle), temperature readout, mode badges (cool/warm/auto). Hero reads like a live system dashboard. | MERIDIAN: newspaper masthead + ticker. SOURA: vertical ledger with glass vessel. KORVA: terminal prompt. Others: split headline + image. |
| **Layout grammar** | Control-panel grammar: `.statusbar` (live pulse) → `.hero-panel` (gauge cluster) → `.readouts` (dark data band) → `.services-grid` (diagnostic modules with colored top-bar) → `.feature` (zig-zag) → `.emergency` (red urgent band). Content reads like an HVAC system status interface. | MERIDIAN: broadsheet multi-column feed. SOURA: vertical ledger + tasting-sheet. KORVA: data-grid + scan lines. Others: alternating section-stack bands. |
| **Typography personality** | **Barlow Condensed** (display, industrial condensed) + **Inter** (body, clean technical) + **JetBrains Mono** (labels, temperature data, system readouts). Industrial control panel voice — precise, technical, urgent. | MERIDIAN: Fraunces/Newsreader/Archivo (newspaper). SOURA: Fraunces/DM Sans (sommelier). KORVA: JetBrains Mono/Sora (terminal). Others: Space Grotesk/Cormorant + Nunito/Jost. |
| **Color logic** | Climate control palette: graphite metal (`--metal`), cool blue (`--cool`), warm orange (`--warm`), frost (`--frost`), emergency red (`--urgent`). 2 temperature axes (cool/warm) + neutral metal. Not a brand ramp — temperature/material reasoning. | MERIDIAN: newsprint paper + kicker-red. SOURA: spring teal + glacier blue + cork. KORVA: graphite + signal-amber. Others: `--primary` brand ramp + neutral ramp. |
| **Motion signature** | Pulse/fan: `.pulse-live` (live status dot), `.reveal` (18px translateY), gauge needle tick. Motion reads like system status — pulse means online, reveal means system activating. | MERIDIAN: clip-path type-set wipe. SOURA: pour-line + bead-pop. KORVA: scan-line wipe. Others: generic opacity + translateY. |
| **Section inventory** | Status bar → Hero panel (gauge) → Readouts band → Service grid (6 modules) → Feature split → Emergency band → Pricing → Testimonials → FAQ → CTA band → Footer. | MERIDIAN: Topbar → Ticker → Masthead → Feed → Rail. SOURA: Micro-bar → Ledger → Proof → Catalogue → Plans. KORVA: Terminal → Eval ticker → Architecture → Benchmarks. |

**Bottom line:** Strip the colors from AERION and any sibling — they share **zero** layout grammar, component set, or motion vocabulary. This reads as an HVAC system control interface, not a marketing site.

---

## Features

- **Live status bar** — pulse-dot animated "SYSTEMS ONLINE" indicator with emergency phone
- **Thermostat gauge hero** — conic-gradient dial with needle, temperature readout, mode badges
- **Readout stats band** — 4-cell dark data band with count-up animation
- **Diagnostic service grid** — 6 service modules with icon, description, colored top-bar
- **Feature split** — zig-zag image/text layout with diagnostic narrative
- **Emergency band** — red urgent CTA with 24/7 dispatch messaging
- **3-tier pricing** — Diagnostic / Maintenance / Installation with featured highlight
- **Testimonials** — 3-column cards with star ratings
- **FAQ accordion** — expandable items with +/- toggle
- **CTA band** — dual-action (schedule + call)
- **Contact form** — service type + equipment type + urgency selects, inline validation, no `alert()`
- **Scroll reveals** — IntersectionObserver with staggered delays (`.d1`…`.d4`)
- **Count-up animation** — stats count from 0 to target on scroll
- **Active nav** — auto-highlight via `location.pathname`
- **Footer year** — `[data-year]` auto-fills current year
- **Reduced motion** — `@media (prefers-reduced-motion)` disables all animation
- **Original imagery** — 14 source images from AirCon (`assets/img/`): `about-1/2/3/4.jpg`, `carousel-1/2.jpg`, `feature.jpg`, `service-1/2/3/4/5/6.jpg`, `icon-01..06-primary.png`

---

## Quick Start

```bash
# No install, no build — just open
open index.html
# or serve locally
npx serve .
```

---

## File Structure

```
ac-repair-html-template/
├── index.html          # Home page
├── about.html          # About / Our Process
├── service.html        # Services detail
├── contact.html        # Contact / Book a Visit
├── assets/
│   ├── css/
│   │   └── base.css    # Bespoke design system (~635 lines)
│   ├── js/
│   │   └── main.js     # Bespoke interactions (~130 lines)
│   └── img/            # 14 original AirCon images
└── README.md           # This file
```

---

## Customization

- **Colors:** Edit `:root` tokens in `assets/css/base.css` — `--cool` (blue), `--warm` (orange), `--metal` (graphite), `--frost`, `--urgent`
- **Fonts:** Swap Google Fonts `<link>` in each HTML `<head>` and update `--font-display/--font-body/--font-mono`
- **Services:** Add/remove `.service-card` items in the `.services-grid` on each page
- **Pricing:** Edit `.plan` tiers in `index.html` — pricing, features, tier count
- **Emergency:** Update the `.emergency` band phone number and response time claims
- **Gauge:** Adjust the thermostat gauge temperature in `.gauge-inner .temp`

---

## Browser Support

Modern evergreen browsers (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+).
Graceful degradation: CSS custom properties, Grid, Flex, `clamp()`, `IntersectionObserver` — all polyfillable if needed.

---

## Credits

- **Images:** Original AirCon source assets (included in `assets/img/`)
- **Fonts:** Barlow Condensed (Impallari Type), Inter (Rasmus Andersson), JetBrains Mono (JetBrains) — all SIL OFL via Google Fonts
- **Icons:** Inline Unicode (❄ 🔥 ⚙ ★ ☰ 📞) — no icon font dependency

---

Let's Build Something Together 🚀
https://tally.so/r/q4q1L9
