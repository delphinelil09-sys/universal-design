---
name: design-saas
description: "SaaS / subscription product site lens. Use when the site markets a software product with plans, trials, or self-serve signup — SaaS marketing sites, pricing pages, feature comparisons, integrations, security and trust pages, product-led growth. Load after design-core has established why the site exists and confirmed the product is subscription software. Replaces design-promo for SaaS: the visitor is buying a promise, not an event. Does not replace design-core; adds subtype-specific priorities, typical failures, layer-by-layer guidance, and audit specifics."
---

# Design SaaS — Subscription Product Sites

A subtype lens for `design-core`. Load this after `design-core` has run its three entry steps and confirmed the product is a subscription software service.

This file does not redefine the eight elements, the four layers, the two modes, or the two phases. It only adds what is specific to SaaS marketing sites.

## Focus

The visitor is buying a **repeated promise**, not a one-time thing. Trust, pricing, and the first minutes after signup matter more than the hero ever will.

Match the site to the go-to-market motion. A product-led product (try it yourself) needs a different site than a sales-led one (book a demo). Generic advice applied to the wrong motion is the costliest mistake in SaaS.

- **Self-serve beats presentation** when the product can be tried: "start free" with a visible next step is stronger than a demo request.
- **Pricing is a discipline, not a section.** Plans must be comparable, one visibly primary, objections answered in place.
- **Trust is placed where doubt happens,** not in the footer: security, compliance, uptime, and integrations appear before forms and price commitments.

## Typical failures

- **Plans that read as identical.** Three cards, equal weight, same voice — the visitor cannot tell which one is for them. Fix: each plan states its difference (limits, seats, support, contract), not just a price.
- **"Start free" with no next step.** The button promises a start; the page never says what happens after (workspace, onboarding, time to first value). Fix: next to the CTA, one line about what happens after the click.
- **Comparison hidden in a modal.** Plan comparison behind a small link is the decision the visitor came for, buried. Fix: comparison is a content unit on the pricing page — a table or a toggle, reachable in one click.
- **Logo mosaic without context.** A row of logos that says nothing about who uses the product or how. Fix: logos grouped or annotated with what they solve.
- **Footer menu with 40 links.** A sitemap dressed as navigation. Fix: navigation for people; depth lives in docs and search.
- **FAQ answering the wrong questions.** Basic "what is X" instead of the real objections — price, migration, cancellation, security. Fix: FAQ is the objection list, spoken aloud.
- **Benefitless CTA.** "Sign up" / "Learn more" everywhere. Fix: benefit-driven labels — "Start free — no card", "See examples built for you".

## Layer-by-layer

**Frame (composition, space).** The frame is the trust route: promise → how it works → why you're safe → the start. Pricing is a decision node, not just another section — the visitor must be able to compare plans where the decision happens. Air gives each block one job; a pricing block that crams table + FAQ + guarantee into one screen reads as pressure, not clarity.

**Body (form, color).** One plan stands out without humiliating the others — distinct form (radius, elevation, weight), muted alternatives. Color is a functional signal: the accent belongs to actions and to the selected state. Twenty pastel fills read as template.

**Surface (texture, typography).** The price is the largest typographic fact on the card; the period ("/mo") is secondary, not equal. Plan descriptions are sentences about outcomes, not feature lists. Texture, if any, supports the product — a screenshot with a real interface beats an abstract illustration.

**Accent (point, line).** Micro-states carry the pricing logic: monthly/annual toggle, hover states, included/excluded marks in feature lists — drawn with different weight, not only color, so they work for color-blind visitors. A "Popular" badge earns its place only if it is true for the audience, not decorative.

## Reading order

SaaS pages follow the trust route, and it does not vary by taste:

1. **Serve** — the promise: what this is, who it's for, what happens after signup (3 seconds).
2. **Prove** — how it works: product in action, screenshots, concrete before/after — not abstractions.
3. **Trust** — security, compliance, uptime, integrations — placed where doubt arises.
4. **Start** — free trial / demo / sales contact — with the next step spoken aloud.

## Audit specifics

Beyond the common grid, these are the SaaS-specific breakages to hunt:

- **Typography → Surface → the price is typographically weak** — "from $X/user/mo" in body size, the period shouting at the number → price is the largest string on the card; the period is muted and secondary.
- **Point → Accent → included / not-included marks are indistinguishable** (same grey check weight) → different shapes and placement, not only color.
- **Form → Body → all plans carry identical visual weight** → elevate the primary plan (radius/elevation/type), let the others recede.
- **Line → Frame → plan comparison lives behind a back-navigation** → comparison table or toggle reachable in one click from the pricing page.
- **Color → Body → accent scattered on decorative elements instead of actions** → accent is a functional signal: actions and selected states only.

## Return to core

For the method (three entry steps, modes, phases, error handling), see `design-core/SKILL.md`. For the marketing filter — which runs here, with conversion leading — see `design-core/references/marketing.md`. For the words on the page, see `design-core/references/copy.md`. For the layers protocol, see `design-core/references/layers.md`.