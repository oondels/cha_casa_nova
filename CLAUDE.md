# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for **Hendrius & Rayane's Chá de Casa Nova** (housewarming party). Event: 25 de Outubro de 2026, Bahia, Brasil.

## Development

No build step. Open `index.html` directly in a browser — or serve it locally:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Architecture

Everything lives in a single file: `index.html`.

**Stack:**
- Tailwind CSS via CDN (`cdn.tailwindcss.com`) with inline config in the `<script id="tailwind-config">` block
- Google Fonts: Noto Serif (headlines) + Manrope (body)
- Material Symbols Outlined (icons)
- Vanilla JS only (no framework, no bundler, no `package.json`)

**Color system:** Material Design 3 tokens are defined in the Tailwind config (e.g. `primary`, `secondary`, `surface`, `on-surface`, `surface-container-*`, `outline-variant`). Always use these tokens rather than raw hex values to stay consistent with the warm earthy palette.

**Page sections (in order):**
1. `#inicio` — Hero with couple name, event date, CTA
2. `#historia` — Our Story (photo + text)
3. `#presentes` — Gift Registry (grid + category filter tabs + progress bar)
4. `#como-funciona` — How It Works (3 steps)
5. `#evento` — Event Details (date, address, RSVP button, map image)
6. Footer + floating back-to-top button

**Gift card states:**
- Available: `bg-tertiary-fixed text-on-tertiary-fixed` badge + active "Presentear" button that fills on hover
- Gifted: `bg-surface-variant text-on-surface-variant` badge + disabled "Indisponível" button; item text uses `/50` opacity

## Pending Features

- Category filter tab interactivity (JS to show/hide cards by category)
- Gift status logic (mark items as gifted, persist state)
- Working RSVP form / confirmation flow
- Mobile hamburger menu for navbar
- Scroll-triggered entrance animations (Intersection Observer)
- Navbar transparency → solid on scroll
