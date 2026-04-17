# Arca AI — Bento Grid Landing Page

> Dark bento grid landing page for an AI SaaS product. Vanilla HTML + CSS + JS. No frameworks, no build tools, no dependencies.

---

## Preview

![Hero](<img width="1919" height="865" alt="desktop-hero" src="https://github.com/user-attachments/assets/b0ee4c24-98f3-4696-a06f-e4330fb93b02" />
)
![Bento Grid](<img width="1915" height="1037" alt="desktop-bento" src="https://github.com/user-attachments/assets/2a2a52c5-2d1f-4487-b20b-7e4f3237f45b" />
)
![CTA](<img width="1919" height="349" alt="desktop-cta" src="https://github.com/user-attachments/assets/dd8ba73e-2ab4-4221-8221-7f96029de680" />
)

---

## What's inside

A single `index.html` file that includes:

- **Sticky navbar** with backdrop blur and animated CTA button
- **Scrolling ticker strip** — seamless infinite loop via CSS animation
- **Split hero section** — large typographic headline + 3 live stat cards
- **Bento grid layout** — 7 cards across a 12-column CSS grid, each a different size and purpose
- **Live chat UI card** — with animated scan line effect
- **Noise texture overlay** — SVG fractalNoise for depth
- **Fully responsive** — tablet (900px) and mobile (560px) breakpoints, hamburger drawer menu
- **Zero JS frameworks** — 14 lines of vanilla JS total (hamburger toggle only)

---

## Stack

| | |
|---|---|
| HTML | Semantic, single file |
| CSS | Custom properties, Grid, Flexbox, `@keyframes` |
| JS | Vanilla, ~14 lines |
| Fonts | Google Fonts CDN (Syne, Instrument Serif, JetBrains Mono) |
| Build | None |
| Dependencies | None |

---

## Design details

**Color palette**

| Token | Value | Usage |
|---|---|---|
| `--bg` | `#0C0C0D` | Page background |
| `--bg3` | `#17171A` | Card background |
| `--lime` | `#C8F135` | Primary accent |
| `--text` | `#F2F2F3` | Body text |
| `--text-sub` | `#888890` | Secondary text |

**Typography**
- `Syne` — headings, nav, UI labels
- `Instrument Serif` — italic decorative accents
- `JetBrains Mono` — tags, ticker, stat labels

**Animations**
- `glow` — lime pulse on primary buttons
- `ticker` — seamless horizontal scroll
- `scan` — vertical scan line on chat card
- `pulse-dot` — live status indicator
- `fadeUp` — staggered page load reveal

---

## Run locally

No setup needed.

```bash
git clone https://github.com/RaduscaWP/Arca-AI-.git
cd Arca-AI-
# Open index.html in your browser
# Or use VS Code Live Server
```

---

## Bento grid structure

```
┌─────────────────────────┬──────────────────────┐
│  Core Features          │  Live Chat UI        │
│  (span 5, row 2)        │  (span 4, row 2)     │
├─────────────┬───────────┤                      │
│  Speed      │  Languages│                      │
│  (span 3)   │  (span 3) │                      │
├─────────────┴─────────────────────┬────────────┤
│  Integrations (span 7)            │  Testimonial│
│                                   │  (span 5)  │
├───────────────────────────────────┴────────────┤
│  CTA Banner (span 12)                          │
└────────────────────────────────────────────────┘
```

---

## What I practiced building this

- CSS Grid with asymmetric column spans and row spans
- Seamless ticker loop (duplicate content + `translateX(-50%)`)
- `backdrop-filter: blur()` for frosted glass nav
- CSS `::before` pseudo-elements for glow effects
- SVG inline data URI for noise texture
- Mobile-first responsive breakpoints
- Hamburger menu with `opacity` + `pointer-events` transition (not `display` toggle)
- Body scroll lock when mobile drawer is open

---

## License

MIT — free to use as reference or practice material.
