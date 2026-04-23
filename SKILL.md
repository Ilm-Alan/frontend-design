---
name: frontend-design
description: Frontend design skill for Claude Code, Codex, and Gemini CLI. Eight anchors with binding CSS tokens, each engineered to escape the AI design default (cream paper, Fraunces, warm ink, red accent, paper grain).
---

# Frontend Design Skill

## The discipline

The AI default for "design a beautiful landing page" is a five-token pattern: **cream-paper surface + Fraunces or Garamond serif + warm near-black ink + one warm-red accent + 2–5% paper grain**. Every ambiguous brief lands there. It is the statistical average of "good design" in training data, and it ships as frontend-design AI-slop — recognisable on sight.

This skill offers eight alternatives, each a concrete escape from those five tokens at the CSS layer. Picking an anchor commits to specific palette, typefaces, and texture — not a vibe. The anchor's *binding signature* is the contract: rendered output either matches the signature or the commitment failed.

There is no "Editorial" anchor. If a brief genuinely earns the default treatment (a print magazine, a literary journal), that output is producible without invoking this skill. The absence of an Editorial label puts a tax on the default choice and clears the path for the alternatives.

---

## 1. Operating Mode

Before writing code, complete this sequence:

1. **Context** — Identify purpose, audience, domain, and content density. State the problem in one sentence.
2. **Anchor selection** — Name three candidate anchors that could fit this brief. One sentence each on what each would do with it. Consult `references/routing.md` to ground candidates in the surface's grammar. Pick the candidate whose grammar most directly serves the brief. State the chosen anchor and the reason in one line.
3. **Differentiator** — Define one memorable anchor-internal move: a signature interaction, a typographic gesture, a layout motif, or a material treatment. One sentence. Describable. Visible in the rendered output.
4. **System** — Commit to the anchor's binding signature exactly. Tune the palette within the anchor's allowed range using `references/palettes.md` for domain-specific tuning. The signature is authoritative — picking Swiss means white + sans + grid, not "some flavor of clean."
5. **Implementation** — Outline structure, then build.

Commit fully to one anchor. Hybridising ("Swiss with Brutalist edge") is a category error — each signature excludes the others by construction.

---

## 2. The Eight Anchors

Each anchor binds specific CSS tokens. Picking the anchor commits to those tokens. If the rendered output uses tokens outside the signature, the commitment failed.

### 1. Swiss

**Surface:** Pure white `#FFFFFF` or neutral `#F7F7F8`. **Typography:** Akzidenz-Grotesk, Helvetica Neue, or Söhne — sans display and body, one family. **Accent:** Swiss Red `#E4002B`, International Orange `#FF4F00`, or Yves Klein Blue `#002FA7` — one, used deliberately. **Structure:** visible grid lines or 1 px hairline rules. Left-aligned typography; asymmetric balance. Numerals as composition elements (dates, folio numbers, page markers set in condensed sans).

**Refuses:** Warm paper, serif display, grain texture, centered typography.

### 2. Industrial

**Surface:** Pitch black `#000000` or warm-black `#0B0C0A`. **Typography:** IBM Plex Mono, JetBrains Mono, or Berkeley Mono *throughout* — mono for display too. **Signal color:** one semantic — green `#00E676`, red `#FF3B30`, amber `#FFB800`, or acid lime `#C6FF4A`. **Structure:** flat; 1 px borders do the work shadows would elsewhere. Tabular numerics locked with `font-variant-numeric: tabular-nums`.

**Refuses:** Serif typography, proportional fonts, warm paper, any grain, decorative shadows, rounded corners.

### 3. Brutalist

**Surface:** Pure primary or anti-primary — `#FF0000`, `#0000FF`, `#FFFF00`, `#000000`, `#FFFFFF`. Pick 2–3, compete equally. **Typography:** system fonts only — Times New Roman, Helvetica, Courier, Arial, system-ui. Mix faces deliberately. **Shadows:** hard offset, no blur — `box-shadow: 8px 8px 0 #000`. **Controls:** native browser — unstyled `<button>`, default `<select>`, underlined blue links that stay blue. Margins crushed; type runs edge-to-edge.

**Refuses:** Webfonts, color tuning beyond pure hex, soft shadows, rounded corners, centered layout.

### 4. Aurora Maximalism

**Surface:** Dark saturated gradient — `linear-gradient` or `conic-gradient` through violet `#5D34D0` → magenta `#FF006E` → cyan `#00F0FF`, or `#3B82F6 → #A855F7 → #EC4899`. **Typography:** Inter Variable, PP Neue Machina, or Sharp Grotesk for oversized display (15–25 vw). **Texture:** mesh gradient as primary surface feature; neon `text-shadow` glow on accents (`0 0 20px <accent>`). **Motion:** spring-physics orchestration, scroll-linked parallax.

**Refuses:** Flat backgrounds, warm paper, restraint, hairline rules as primary structure.

### 5. Chaotic Maximalism

**Surface:** Clashing palette — pastels *and* neons in the same composition. Hot pink `#FF71CE` + acid yellow `#DFFF00` + cyan `#00FFFF` + any third. **Typography:** mixed faces deliberately colliding — 3+ faces from different registers on the same page. **Texture:** patterns on every surface (squiggles, dots, zigzags, checker — SVG or `repeating-linear-gradient`). Oversized display crashing against busy ground.

**Refuses:** Coherent palette, single typeface, whitespace as structural element, 60/30/10 dominance.

### 6. Retro-Futuristic

**Surface:** Pitch black `#0A0014` or deep navy-black. **Typography:** period-specific — VT323 (CRT), Orbitron (synthwave), Space Mono (cyberpunk), Monoton (Miami-neon), Press Start 2P (arcade), IBM Plex Mono (terminal). **Accent:** neon pair — magenta `#FF006E` + cyan `#00FFFF` (synthwave) or phosphor green `#00FF41` + amber `#FFB000` (terminal). **Texture:** CRT scanlines via `::before` `repeating-linear-gradient` overlay, or chromatic aberration (`text-shadow: 2px 0 #FF0000, -2px 0 #00FFFF`), or both. Glow committed.

**Refuses:** Flatness, modern sans-serifs (Inter, Söhne), paper surfaces, absence of texture.

### 7. Organic

**Surface:** Earth tones — sage `#8B9D83`, clay `#B08B6E`, terracotta `#C66B3D`, ochre `#C08E3A`, moss `#606C38`. When a light surface is needed: sand `#E8DCC7` or oat `#D4B895`. **Never cream `#F0-F8` warm-paper range.** **Typography:** humanist serif (Freight, Caslon, Fraunces — Fraunces is restricted to this anchor only) or warm geometric sans (Greycliff, Epilogue, Recoleta). **Structure:** rounded corners 16–32 px. **Texture:** grain at 1–3 % via SVG feTurbulence. **Motion:** gentle ease 300–500 ms, breathing animations on hero elements.

**Refuses:** Cream backgrounds (warm-tinted `#F0+`), cold greys, pure whites, pure blacks, hard rectangles.

### 8. Lo-Fi

**Surface:** Paper-yellow `#E8E0C0` or `#EDE4CF` — more saturated than cream. **Typography:** mixed system fonts on the same page (Times + Helvetica + Courier colliding deliberately). **Structure:** rotated elements (2–8° off-grid via `transform: rotate`). **Texture:** halftone dot transitions (SVG pattern or `radial-gradient` tile) on imagery; Risograph misregistration (2–4 px RGB channel offset via `text-shadow: 3px 0 #FF006E, -3px 0 #00FFCC`). SVG staple, tape, torn-edge elements.

**Refuses:** Precision, single typeface, smooth motion, rectangles squared to the grid, cream (it is specifically paper-yellow, more saturated).

---

## 3. Output Contract

Every implementation delivers:

- **Stated direction** — A short preamble in a designer's prose before the code, naming: chosen anchor, the three-candidate deliberation outcome, the differentiator, and the key palette / typefaces / texture choices pulled from the signature. Written with conviction, not as a checklist.
- **Signature fidelity** — The rendered CSS matches the anchor's binding signature at the token level. If Swiss is chosen, the CSS contains no warm paper, no Fraunces, no grain. If Industrial is chosen, every typeface declared is monospace. Signature violations mean the commitment was performative.
- **Differentiator visible** — The one memorable move is implemented in the rendered output, not merely described.

---

## 4. Intention Check

Before delivering:

- **Anchor deliberation** — Did three candidates get named and reasoned about, or did the first instinct win?
- **Signature fidelity** — Do the rendered tokens match the anchor's binding signature? Did cream-paper-Fraunces-grain ship under a different label?
- **AI-slop check** — Does the output look like the statistical average of "AI-produced design"? If yes, the signature was not held.
- **Differentiator visible** — Is the memorable anchor-internal move actually rendered?
- **Hybrid resistance** — Was one anchor held, or did the execution drift into "Swiss with Brutalist edge"?

Intention in every choice. The anchor binds identity at the CSS layer, not just in the preamble.
