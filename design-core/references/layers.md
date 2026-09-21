# Layers — Movement Protocol

The eight elements do not live at the same level. They sit on four layers, ordered by strength of influence. Movement goes from strongest to weakest.

## The four layers

| Layer | Elements | Role | Strength |
|---|---|---|---|
| **Frame / Каркас** | Composition, Space | Where things sit, how much air | Strongest |
| **Body / Тело** | Form, Color | Silhouettes and tone inside the frame | Medium |
| **Surface / Поверхность** | Texture, Typography | Tactility and voice on the surface | Weaker |
| **Accent / Акцент** | Point, Line | Details, dividers, icons | Weakest |

## Movement rules

1. **Move top-down.** Frame → body → surface → accent. Each layer constrains the ones below it. You cannot decide color before you know the composition it sits in.

2. **Stronger wins.** When a weaker layer conflicts with a stronger one, the stronger wins and the weaker is re-decided. Do not compromise the stronger layer to save the weaker.

   Concrete example: an acid accent color (body) breaks a calm composition (frame). The frame wins. The accent is re-picked to fit the frame — not the other way around.

3. **Return allowed, downward never.** You may go back to a stronger layer to revise it if a weaker layer reveals a problem. You may not fix a weaker layer by damaging a stronger one.

## Why this order

This is not a checklist. It is a dependency graph. The frame decides where attention goes. The body decides what the attention lands on. The surface decides how it feels. The accent decides the last 5%. Reverse the order and you get decoration on top of a broken structure — which is the most common failure mode of AI-generated design.

## In the two modes

- **Creation** moves top-down through the layers. See `generation.md`.
- **Audit** does not use this order. It reads the artifact across all eight elements at once using the grid in `audit-grid.md`, finds conflicts, and fixes them. A broken accent is meaningless if the frame is also broken — the grid finds both.

## Conflict resolution example

A landing page hero: the designer wants a large animated gradient (body/color) with a headline over it. The frame says the headline needs a stable background to read against. Options:

- Kill the gradient → frame wins, body re-decided. ✅
- Keep the gradient but add a scrim behind the headline → both satisfied. ✅
- Keep the gradient as-is and hope the headline reads → frame damaged to save body. ❌

The third option is what happens when the protocol is skipped.