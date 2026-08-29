# AERION — AC &amp; Climate Comfort (Redesign)

A premium, framework-free redesign of the **AirCon · AC Repair Website Template** (source zip: `source/AirCon.zip`).

> Reimagined as **AERION**, a fictional licensed HVAC company. English / LTR only.

## What changed
The original was a single-page Bootstrap-based HTMLCodex AC-repair template with placeholder copy. This rebuild:

- **Drops all frameworks** — pure semantic HTML, hand-written CSS (token-driven design system), vanilla JS. No Bootstrap, no Tailwind, no build step.
- **New brand identity** — "AERION", a local, licensed HVAC company with its own voice.
- **New Design DNA** — airy "climate comfort" aesthetic, glacier cyan (cooling) + warm orange (heating) dual accent, Sora × DM Sans, soft blobs and floating badges.
- **Real, specific copy** — no Lorem Ipsum; believable services, prices-by-quote, stats and testimonials.
- **Single, complete page** — faithful to the original one-page template, with anchored nav (home, services, why-us, process, installs, contact).
- **Motion with purpose** — scroll reveals, count-up stats, floating badges, all respecting `prefers-reduced-motion`.
- **Accessibility** — semantic landmarks, visible focus, keyboard nav, ARIA on the mobile toggle, reduced-motion support.

## Design DNA (summary)
- **Philosophy:** comfort you can trust — upfront pricing, owned trucks, real warranty.
- **Personality:** Local · Licensed · Reliable · Friendly.
- **Palette:** cool off-white `#F2F7F9` (bg), white surface, deep navy `#0E1B2A` (ink), glacier `#0EA5C9` (cooling accent), warm `#FF7A3C` (heating accent).
- **Type:** Sora (display) × DM Sans (body).
- **WOW moment:** split hero with soft gradient blobs, a framed photo, and floating "24/7 / Licensed" badges.

## Page
| File | Purpose |
|------|---------|
| `index.html` | Single page — hero, trust marquee, services, why-us, process, installs, testimonial, contact form, CTA, footer |

## Structure
```
ac-repair-html-template/
├─ index.html
├─ assets/
│  ├─ css/base.css      # design tokens + components + motion + responsive
│  └─ js/main.js        # nav state, mobile menu, reveals, counters, form
└─ README.md
```

## Run it
Open `index.html` in a browser — no server or install required. Imagery uses seeded `picsum.photos` placeholders; swap `src` values for real photography when available.

## Notes
- Original assets were used for reference only and are **not** copied into this folder.
- The GitHub-Pages automation step described in the project workflow is handled separately (not generated here).
