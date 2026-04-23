---
name: frontend-design
description: Frontend design skill for Claude Code, Codex, and Gemini CLI. Demands a specific reference, a governing move, and an opinion before the code. Refuses to ship generic.
---

# Frontend Design Skill

## The discipline

Bad design is generic. Good design is specific. The difference is not technique — technique is table stakes. The difference is **commitment**: naming, before a single line of code, the specific thing this design is trying to be.

"Editorial" is not a commitment. "GT Sectra display against Söhne body, Wallpaper magazine March 2024 column grids, one accent warmer than any other site in the category" is a commitment.

The difference between these two sentences is the difference between a defaulted approximation and a design.

---

## Before you touch code

Answer these four questions in the output preamble. Each demands a specific named answer. No categories. No "-ish." No hedging.

### 1. What is this surface for?

Not the brand. Not the industry. What does this page *do* for the person reading it? One sentence. If you need two, you don't understand the brief yet.

### 2. What specific design does this remind you of?

Name a real, specific thing: a site (URL), a designer's work, a magazine spread, a movie title sequence, a record sleeve, a software tool. **One reference.**

If the answer is a category ("Editorial," "Swiss," "a luxury brand"), go back.

If the answer is "Linear or Vercel," go back — pick one.

The reference must be specific enough that someone could look it up.

### 3. What is the governing move?

Every good design has one move you could describe in a sentence — the move that makes someone remember the design a month after they saw it. Not the palette. Not the typeface. The *move*.

If you cannot name one, the output will be generic. Go back.

### 4. What would a senior designer raise an eyebrow at?

The bold choice. Not tasteless — opinionated. Something a polished, defensible design would never do.

If there is nothing a senior designer would raise an eyebrow at, the design has no opinion. Add one.

---

## Constraints

- **No hybrid directions.** Pick one archetype, one mode. "Editorial with a brutalist edge" is two directions. Name one.
- **No rule-of-three differentiators.** If the design has three memorable moves, none is memorable. One.
- **Typography is not a governing move unless it is.** Beautiful type is table stakes, not an opinion.
- **Default to no texture.** Grain, scanlines, glass blur, noise — each is a specific commitment, not a finishing touch. If the named reference has no paper grain, neither does the output.
- **If the brief calls for raw, anti-design, DIY, or punk:** sanitized execution is a category error. The polish *is* the betrayal. System fonts, hard offset shadows, snap motion, deliberate misalignment — commit to the anti-craft. "Polished Brutalism" is an oxymoron.

---

## Override the first instinct

Ambiguous briefs attract refined-editorial by default. Override that attraction.

Whatever the obvious safe answer is, ask what the design would be if that answer were unavailable. The override answer is usually the better one. Return to the obvious answer only when the override is worse on reflection, not when the override is just less comfortable.

---

## Output

A single-file HTML document with embedded CSS, preceded by the four answers above, written with a designer's voice — direct, committed, specific.

The four answers must be visible in the rendered output. Someone reading the preamble and opening the file should recognise every commitment on the page. If they cannot, nothing has actually been committed to.

A test of commitment: if the output could have been produced by any competent assistant following a generic "design a beautiful landing page" instruction, the commitments were not hard enough. Push further.
