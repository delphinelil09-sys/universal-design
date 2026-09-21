# Audit Grid

Used in **audit mode**. Reads all eight elements at once, not in layer order. The goal is completeness — find everything broken before fixing anything.

## The grid

| Element | What's there | What it should be | What's wrong |
|---|---|---|---|
| **Point** | Icons, bullets, dividers | Consistent size, aligned to text baseline | Mixed sizes; dots that don't anchor anything |
| **Line** | Rules, borders, underlines | Consistent weight, purposeful | Decorative rules with no meaning; too many |
| **Form** | Buttons, cards, crops | One radius system, one silhouette logic | Mixed radii; button shapes fighting cards |
| **Color** | Background, surface, text, accent | 60-30-10 distribution; contrast ≥4.5:1 | Grey-on-grey; accent used everywhere; no hierarchy |
| **Texture** | Backgrounds, shadows, grain | Supports depth without noise | Gradients as decoration; soft shadows on everything |
| **Space** | Margins, padding, gaps | Scale 4/8/12/16/24/32 | Random values; tight where it should breathe |
| **Typography** | Headings, body, labels | Explicit scale; ≤80 chars per line | Too many sizes; unreadable body; decorative labels |
| **Composition** | Grid, alignment, reading order | One alignment system; clear reading order | Elements "walk"; no clear primary / secondary |

## Objective checks (Phase 1)

These are non-negotiable. Fix without asking.

- **Contrast** — body text ≥4.5:1; large headings ≥3:1.
- **Click zones** — ≥44×44px on mobile.
- **Body text** — ≥16px on mobile.
- **Focus** — visible focus indicator on every interactive element, not only on hover.
-- **Spacing scale** — values come from 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64, not random.
- **CTA hierarchy** — one clear primary, everything else visibly subordinate.
- **Alignment** — one system; nothing off-axis without reason.
- **Fill** — empty space is air (working) or a hole (broken). Air separates groups; a hole is space that serves nothing.

## Finding format

Write every finding in this shape so fixes are traceable:

```
Element → Layer → Problem → Fix
```

Example:

```
Color → Body → accent #FF6B6B on #FFFFFF fails contrast at 3.1:1
→ darken to #C43D3D (4.7:1), or move the accent to a dark surface
```

Example:

```
Space → Frame → section padding is random: 22px, 30px, 18px, 44px
→ snap to scale: 24px, 32px, 16px, 48px
```

## What the grid does not do

The grid finds what is broken. It does not generate character. After the grid is cleared, the site is correct — but it is not yet distinctive. That is Phase 2, and it requires the user's idea and reference. See `design-core/SKILL.md`.
