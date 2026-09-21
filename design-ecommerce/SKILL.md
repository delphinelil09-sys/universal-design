---
name: design-ecommerce
description: "Ecommerce / product site lens. Use when the site's purpose is to sell physical or digital products — online stores, product detail pages, catalogues, shopping cart flows. Load after design-core has established why the site exists and confirmed the goal is purchase. Does not replace design-core; adds subtype-specific priorities, typical failures, and layer-by-layer guidance."
---

# Design Ecommerce — Stores & Product Pages

A subtype lens for `design-core`. Load this after `design-core` has run its three entry steps and confirmed the goal is purchase.

This file does not redefine the eight elements, the four layers, the two modes, or the two phases. It only adds what is specific to ecommerce sites.

## Focus

Usability beats beauty, but a product card can be a piece. The purchase path runs without friction — every step the visitor must take is one step too many. Trust is visible early: shipping, returns, guarantees, reviews appear before the visitor has to wonder. Comparison between products is easy, not hidden behind a filter maze.

Marketing leads by default. The floor is non-negotiable: contrast, click zones, focus, body size.

## Typical failures

- **Indistinguishable cards.** Every card looks the same, so no card is remembered. Fix: let the product dictate the card's hierarchy — image, name, price, not a uniform template.
- **Price or availability buried.** The two facts a buyer needs first are the two facts hidden last. Fix: price and availability are visible on the card, not only on the detail page.
- **Heavy filters.** Ten filter dimensions, none applied by default, all distracting. Fix: filters reduce results, not attention.
- **Checkout that suddenly complicates.** The cart works, then step 2 asks for a phone number, then step 3 requires an account. Fix: every step past "add to cart" must justify its existence.

## Layer-by-layer

**Frame (composition, space).** The card grid is stable — one rhythm, even gaps, no surprises. Space between cards is consistent so the eye can scan, not re-orient per row. Navigation (categories, search) is a working tool, not a hero.

**Body (form, color).** Color serves the product. The palette recedes — the products provide the color. Button forms are unambiguous: "add to cart" is a distinct shape, "add to wishlist" is visibly secondary. Radius system is one token, applied consistently.

**Surface (texture, typography).** Price and product name are typographically clear — the two things that must be readable at a glance. Description text is readable at body size, not shrunk to make room. Product images are treated as surfaces, not just thumbnails.

**Accent (point, line).** The primary action is obvious everywhere it appears. Icons (cart, search, wishlist) are consistent in weight. Dividers and rules stay out of the way unless they separate distinct sections.

## Reading order

The ecommerce flow has three distinct reading orders, and each is optimized for its own step:

1. **Browse** — categories are scannable, products are distinguishable, price/availability visible.
2. **Decide** — detail page answers the buyer's real questions (material, size, delivery, returns) in the order they arise.
3. **Buy** — checkout confirms, doesn't interrogate. Every field has a visible reason.

## Return to core

For the method, see `design-core/SKILL.md`. For the marketing filter (which runs here), see `design-core/references/marketing.md`. For the layers protocol, see `design-core/references/layers.md`.