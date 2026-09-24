---
name: design-core
description: "Universal method for designing, auditing, and elevating websites. Use whenever the user works on a site — landing page, portfolio, ecommerce, info site, SaaS — mentions redesign, 'make it look better', 'why does my site look generic', 'audit my site', 'why isn't this converting', or asks for a site that doesn't look AI-generated. Routes to one of five subtype skills (design-promo, design-portfolio, design-ecommerce, design-info, design-saas) after establishing why the site exists. Covers two modes (audit / creation) and two phases (floor / ceiling)."
---

# Design Core

The universal method for working on websites. This skill is the entry point. It establishes context, asks the right question, and routes to a subtype lens. It does not design anything by itself — it makes sure the work starts in the right place.

Scope: **websites only.** Not business cards, posters, decks, apps, or dashboards.

## Three entry steps

Before touching design, walk these three steps in order. They are the same whether the task is audit or creation.

### 1. Observation

Establish three facts. If any is unclear, ask.

- **Artifact** — is there a ready HTML, a screenshot, a URL, or only a brief?
- **Subtype** — is this promo, portfolio, ecommerce, info, or saas (subscription software)? (See routing below.)
- **Task** — is this create, fix, or elevate?

### 2. Why

Do not start design work until you know why the site exists.

- What is it for — sale, impression, explanation, self-declaration?
- Who is the audience?
- What should happen after someone views it?

The answer decides **who leads**:

| Goal | Who leads |
|---|---|
| Sale, signup, conversion | Marketing leads |
| Impression, character, work | Design leads |
| Explanation, trust, structure | They cooperate — design serves clarity |

### 3. Routing

Load the subtype lens that matches the site. If the subtype is not obvious (a hybrid — e.g., a studio site that both shows work and sells services), **ask the user**: "Is this more about impression or about sale?" Then load the leading subtype, and pull in the second only for the sections that need it.

## The running context

From entry to done, keep these five facts in mind. They are the context the lens builds on — a lens never restarts the method, it adds to it:

1. **Artifact** — HTML, screenshot, URL, or brief?
2. **Subtype** — which lens is leading?
3. **Who leads** — marketing (sale), design (impression), or cooperation (explanation)?
4. **Mode** — audit or creation?
5. **Phase** — floor (fixed), ceiling (user's direction), or both?

State them aloud when the lens loads, so the user can correct a wrong assumption early. If a later decision contradicts one of these five, the context wins and the decision is re-made.

## Two modes

The entry step decides which tool runs.

| Mode | When | Tool | Phase weighting |
|---|---|---|---|
| **Audit** | User hands you an artifact | Grid — read all eight elements at once, hunt for conflicts | Phase 1 = main work, Phase 2 = optional |
| **Creation** | User hands you a brief | Layers — move top-down | Phase 1 = quick check, Phase 2 = main work |

**Audit** does not follow the layer order. It reads the artifact across all eight elements simultaneously, finds what's broken, and fixes it. See `references/audit-grid.md`.

**Creation** moves through layers from strongest to weakest: frame → body → surface → accent. See `references/layers.md` and `references/generation.md`.

## Scope discipline

Read the request before choosing scope.

- **Vague request** — "look at my site", "review this", "what do you think", "any suggestions". Run the **full floor audit** first: all eight elements, floor findings, format `Element → Layer → Problem → Fix`. Then offer Phase 2 separately. Do not jump straight to character suggestions.
- **Specific request** — "check the signup form", "what's wrong with the hero", "fix the contrast". Do exactly that. **Do not expand scope.** Do not run a full audit unless the user asks for one.

Examples:
- "Check out my website" → full audit, all eight elements, floor first.
- "What's wrong with hero?" → hero only. Do not audit other sections.
- "Check the contrast." → contrast check only. Do not expand to other Color findings.

## Two phases

Every task has a floor and a ceiling.

### Phase 1 — Floor (autonomous)

Fix what is objectively broken. Do not ask permission — fix it. What counts as broken:

- **Contrast** — text against background below 4.5:1 (3:1 for large headings).
- **Click zones** — interactive targets smaller than 44×44px on mobile.
- **Body text size** — below 16px on mobile.
- **Focus** — no visible focus indicator on interactive elements (not only hover).
- **Spacing scale** — random values instead of 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- **CTA hierarchy** — no clear primary / secondary / tertiary distinction.
- **Alignment** — mixed systems with no reason; elements that "walk".
- **Fill** — empty space that reads as a hole, not as air.

When Phase 1 is done, the site is **correct**. Not beautiful — correct. The user may stop here, and that is a complete outcome.

### Phase 2 — Ceiling (never autonomous)

Do not invent a concept. Phase 2 requires the user to provide:

1. **An idea** — what should this express, what character.
2. **A direction** — a reference, an example, "like X but Y".
3. **Material** — photos, textures, brand elements, if any.

With those, expand the idea into concrete decisions using the protocol in `references/ceiling.md`: decompose the reference by elements, extract the gesture (one sentence), translate top-down through the layers. Without them, Phase 2 does not run. Say so plainly: "Character cannot be chosen for you — give me a direction, or the site stays at the floor."

**Phase 2 never runs on a site that failed Phase 1.** Correctness first, character second.

## References

References are **not** pasted into this file. To load one, read its file with your available read/file tool — never guess its content. Load on demand; do not read them all at once.

- `references/elements.md` — the eight elements as vocabulary. Load when first speaking about design vocabulary.
- `references/layers.md` — top-down movement protocol. Load in creation mode.
- `references/audit-grid.md` — diagnostic grid. Load in audit mode.
- `references/generation.md` — the "0 to 1" process. Load in creation mode.
- `references/ceiling.md` — Phase 2 protocol: idea + reference → concrete decisions. Load in creation mode when the user brings a direction.
- `references/marketing.md` — marketing as a filter layer. Load when the goal is sale.
- `references/copy.md` — words as a design element; the textual slop filter. Load in audit and creation whenever text is written or assessed.
- `references/trends-2026-Q3.md` — dated snapshot of current patterns. Load when the user asks for "current" or "modern"; check freshness.

## Subtype routing

- **promo** (landing pages, product launches, service promos) → load `design-promo`.
- **portfolio** (designer, photographer, agency, artist) → load `design-portfolio`.
- **ecommerce** (stores, product pages, catalogues) → load `design-ecommerce`.
- **info** (corporate, documentation, content-heavy) → load `design-info`.
- **saas** (subscription software, pricing, product-led growth) → load `design-saas`. For subscription products this replaces promo — the visitor is buying a promise, not an event; pricing and trust carry the page.

If the site is a hybrid, ask first, then load the leading subtype.

## Error handling

1. **No stated goal.** Do not guess. Ask "why does this exist?" and offer a hypothesis ("looks like a landing page for sale — right?") to make it easy to confirm or correct.

2. **Ambiguous subtype.** Ask: "impression or sale?"

3. **"Make it beautiful" with no reference.** Phase 2 does not run. Explain why and ask for a direction.

4. **HTML too large.** Work by sections — first screen, navigation, cards — or ask for the key fragments.

5. **User asks to break the floor.** Aesthetic rules (spacing, alignment, rhythm) may be broken at the user's will. Accessibility rules (contrast, click zones, focus) may not. The floor exists for people, not taste.

6. **User doesn't know a term.** Explain using their own site: "the frame of your site is this block — and it's broken here."

## What this skill is not

It is not a checklist. It is not a style. It is not a set of patterns to apply. It is a method: establish why, choose the mode, move through the layers or the grid, and stop at the floor unless the user brings an idea.
