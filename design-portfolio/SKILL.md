---
name: design-portfolio
description: "Portfolio / studio site lens. Use when the site's purpose is to impress through the work itself — designer, photographer, illustrator, agency, artist portfolios. Load after design-core has established why the site exists and confirmed the goal is impression, not conversion. Does not replace design-core; adds subtype-specific priorities, typical failures, and layer-by-layer guidance."
---

# Design Portfolio — Portfolio & Studio Sites

A subtype lens for `design-core`. Load this after `design-core` has run its three entry steps and confirmed the goal is impression, not conversion.

This file does not redefine the eight elements, the four layers, the two modes, or the two phases. It only adds what is specific to portfolio sites.

## Focus

The work is the center. Everything else is silence around it. Character matters more than conversion. The first screen is a statement, not a catalogue — it says what world the visitor has entered, not what's for sale. Navigation is subordinated to the work, not the reverse.

Design leads by default. Marketing is not active as a filter here, though a clear path to contact still matters.

## Typical failures

- **Work drowns in decoration.** Ornamental backgrounds, animated intros, parallax layers fighting the pieces. Fix: strip until the work is the loudest thing on the page.
- **Grid kills varied formats.** A rigid grid imposes one aspect ratio on portraits, landscapes, and square pieces. Fix: let the grid flex per project, or use a masonry approach that respects each piece.
- **Animation for animation's sake.** Every hover triggers a transition, every scroll triggers a fade. Fix: one orchestrated moment (page load or first reveal), motion that answers action otherwise.
- **No path to contact.** Character without a way to reach you is a dead end. The contact path must be visible, not hidden in the footer.

## Layer-by-layer

**Frame (composition, space).** The composition serves the work. Space is generous — the work needs air or it reads as an inventory. The first screen is a statement: a single image, a single line of type, or one crafted moment. The rest of the page holds the work in a rhythm, not in a grid.

**Body (form, color).** Color is restrained. The work provides the color — the site's palette should not compete with it. Form is soft where it needs to recede, sharp where it needs to frame. Radius is a decision, not a default.

**Surface (texture, typography).** Typography carries much of the character. The typeface is chosen, not defaulted — it is part of the site's voice. Type scale is deliberate; a portfolio can afford large display sizes because it has few words.

**Accent (point, line).** Minimal. Dividers and rules are used only if they encode structure. Icons, if present, are custom or drawn from a single coherent set. The accent never argues with the work.

## Reading order

Portfolio reading order is about immersion, not conversion:

1. Statement (first screen — what world is this)
2. Work (the pieces, in a rhythm the visitor can move through)
3. Contact (the path out)

Navigation may live at the side, in a persistent menu, or as a quiet top bar — but it never occupies more visual weight than the work itself.

## Audit specifics

Beyond the common grid, these are the portfolio breakages to hunt:

- **Form → Body → the grid forces one aspect ratio on mixed work** (portraits, landscapes, squares) → flex the grid per project, or use a masonry approach that respects each piece.
- **Color → Body → the site's palette competes with the work** → the work provides the color; the site's palette recedes.
- **Typography → Surface → project descriptions set below readable body size** → 16px floor and air, even over images.
- **Line → Accent → frames and rules around every piece add noise** → borders only where they carry structure.
- **Space → Frame → no path to the next project** ends the visit → each project points onward; contact is part of the frame.

## Return to core

For the method, see `design-core/SKILL.md`. For the layers protocol, see `design-core/references/layers.md`. Marketing does not run as a filter here, but a path to contact is not optional — it is part of the frame.