# Universal Design Skill — Eval Set

Four eval prompts to run after the skill set is installed.

## How to run

**Option A — Chatbox, new session (recommended).**
Install the five skills into the Chatbox skills directory (`C:\Users\TANSHI\AppData\Roaming\xyz.chatboxapp.app\skills`), start a fresh session, and paste each prompt. Do NOT mention the eval in the prompt — just paste the user-facing text. Watch whether the skill triggers, which mode it picks, which subtype it routes to.

**Option B — skill-creator cycle.**
Use the skill-creator skill's iteration loop. Place this eval set at `evals/evals.json` inside `design-core/` and run the standard with-skill / baseline comparison.

## What to watch

For each eval, check every assertion in `evals.json`. The important failure modes:

- **Eval 1 fails** if the skill invents a concept without being asked (that's Phase 2 leaking into Phase 1).
- **Eval 2 fails** if the output is the default cream + serif + terracotta — the skill didn't use the reference as source material.
- **Eval 3 fails** if the skill starts designing instead of asking. This is the most important eval — it tests the hard gate.
- **Eval 4 fails** if the skill silently picks one subtype and proceeds. The whole point is to ask.

## Baseline

For each prompt, also produce what a plain session (no skill) would output on the same prompt. Compare:

- Does the skill find issues the baseline missed?
- Does the skill avoid defaults the baseline fell into?
- Does the skill ask the questions the baseline skipped?

If the skill and the baseline look the same, the skill is not pulling its weight.

## Freshness

Run this eval set once per quarter, alongside a snapshot update. Trends change; the eval should change with them.