# DESIGN.md — "Systems Reference" world

Durable visual decisions for rgmamani.github.io. This replaces the previous w3schools "Resume/CV" template (recorded here only as anti-reference).

## Direction: the CV as an engineering reference document
A systems architect's own artifact — a technical **reference sheet / architecture document** — turned into the portfolio. The visitor reads Gabriel through the grammar he works in daily: drafting title block, a precise grid, dimension/annotation marks, monospaced coordinates and codes, and a career rendered as a **system timeline** (a topology of roles), not a flat list. Deliberately NOT the terminal-hacker cliché (no dark neon mono costume) and NOT warm-cream-serif.

## Color strategy: Restrained (cool technical paper + ink + one accent)
Light surface, chosen from the use scene: a recruiter scanning long CV text on a laptop in daylight. Accent is a precise **blueprint blue** (doubles as an Azure nod), used as field fills for the current role and interactive elements — not scattered.

Tokens (durable roles; exact hex may refine in build):
- `--paper` cool off-white ground (NOT cream)
- `--sheet` white sheet/card surface
- `--ink` near-black cool for primary text
- `--ink-2` / `--ink-3` secondary / muted (cool-tinted, not flat gray)
- `--line` / `--line-2` drafting rule lines (hairline grid, dimension lines)
- `--accent` blueprint blue (regions + interaction); `--accent-ink` darker for hover; `--accent-wash` pale fill
- `--redline` engineering annotation red — used ONLY for revision/marginalia ticks, never as body accent

## Type
- **Archivo** — display + UI. Wide tracking for title-block labels; strong weight/size steps carry hierarchy.
- **Spline Sans Mono** — data only: dates, codes (§01…), coordinates, measured values, dimension labels. Mono is for measurement, never decoration.
- Fallbacks: `system-ui, sans-serif` and `ui-monospace, monospace`. Fonts via Google Fonts with `preconnect`.

## Signature devices (the world's grammar)
- Drafting **title block** header: name as H1 at display scale, role, live experience field, location, "sheet 1/1", revision/date — as labeled fields.
- Hairline **grid + corner crop marks** framing the page.
- Section headers as document codes: `§01 SUMMARY`, `§02 EXPERIENCE`, `§03 STACK`, `§04 EDUCATION` (mono kicker — a chosen system code, not an eyebrow-everywhere).
- **System timeline** for work history: a vertical spine with nodes; the current role is a highlighted module (accent field); roles 2006–2014 collapse into an `ARCHIVE` disclosure so recent/senior work leads.
- Skills as a **calibrated spec meter** with tick marks and the numeric value shown as mono data (honest to his stated values), not a vague progress bar.
- Contact as a document footer/stamp with a real primary action (`mailto:`) and `window.print()` "save as PDF" (no fake download).

## Motion
One authored moment: on load, the grid/title-block settles and the timeline spine draws downward with a staggered node reveal (exponential ease-out, from an already-visible default). Bounded; fully disabled under `prefers-reduced-motion` while preserving all content and state.

## Non-negotiables
- Semantic landmarks (`header`/`main`/`section`/`footer`), single `h1`, ordered headings, `lang="en"`, `aria-label` on icon links, `focus-visible`, real `alt`.
- No w3.css, no Font Awesome — self-contained CSS, inline SVG icons drawn in a consistent 1.5px drafting stroke.
- Static, GitHub-Pages-deployable. Relative asset paths.

## Anti-references (what this world refuses)
Terminal/hacker dark-neon; percentage progress bars as decoration; same-size icon+heading+text cards as page structure; gradient text; glass/blur decoration; the w3schools template it replaces.
