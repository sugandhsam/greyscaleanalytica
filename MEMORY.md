# MEMORY — Greyscale Analytica

Company landing page for Greyscale Analytica, a market intelligence product for corporate strategy teams.

## Stack
- Language: HTML + vanilla JS
- Framework: none (static prototype)
- Package manager: none (Tailwind via CDN)
- Database: none
- Testing: none yet (visual check in a browser)
- Styling: Tailwind CDN + tokens from `docs/Quantum-Particulate-Render-Matrix-DESIGN.md`

## Invariants
- The only design language for this repo is `docs/Quantum-Particulate-Render-Matrix-DESIGN.md` (with `docs/Quantum-Particulate-Render-Matrix.html` as its reference build). No house Chalk theme, no Shadcn Blocks style, no Vanguard, no colors, fonts, radii or shadows from anywhere else.

## Decisions
- **What:** Use the Quantum Particulate design language for this repo, replacing the global `design.md` house default (`base-maia` + Chalk).
  **Why:** Sam's explicit call for this project (2026-10-07).
  **Rejected:** Vanguard Partners language — a first prototype was built with it and Sam didn't like it (2026-10-07). Vanguard layout with Chalk tokens — Sam wants one design doc, unmixed.
- **What:** Accent color is `#F1CD26` (yellow), replacing the doc's primary `#8B5CF6`. Everything else stays from the Quantum doc. Text on the accent is `#18181B`, never white, and the accent isn't used for text on white (too low contrast).
  **Why:** Sam's override, 2026-10-07.
- **What:** Headline uses Geist Mono (Google Fonts, 300), set as three fixed lines. Everything else stays Inter.
  **Why:** Sam's override, 2026-10-07; the Quantum doc defines Inter only.
  **Rejected:** Instrument Serif (tried, Sam didn't like it), Newsreader (brings back the rejected Vanguard look), Fraunces (too warm for the quant tone).
- **What:** Landing page is a single hero section, no sub-sections.
  **Why:** Sam's call after reviewing a multi-section version (2026-10-07).
  **Rejected:** Platform / Method / Brief / Teams sections below the hero.
- **What:** First prototype is one static HTML file, `prototype/index.html`.
  **Why:** Fastest way to iterate on the look; matches the reference build.
  **Rejected:** Next.js + Shadcn Blocks for now — slower to a first look; revisit for production.
- **What:** Audience is corporate strategy, product, corporate development and leadership teams (business market intelligence, not financial markets).
  **Why:** Sam's answer, 2026-10-07.
