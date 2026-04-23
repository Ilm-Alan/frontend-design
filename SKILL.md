---
name: frontend-design
description: Frontend design skill for Claude Code, Codex, and Gemini CLI. Eight aesthetic anchors, each locking palette, typography, and texture to specific CSS tokens. Pick one per brief.
---

# Frontend Design Skill

Eight anchors. Each is a distinct aesthetic territory locked to specific CSS tokens. Pick one per brief. Match its tokens.

---

## 1. How to work

Before writing code, run this sequence:

1. **Context** — Identify purpose, audience, domain, content density. State the problem in one sentence.
2. **Anchor selection** — Name three candidate anchors. Include at least one that isn't the obvious fit — a Brutalist SaaS dashboard or a Retro-Futuristic restaurant site has more charge than the safe pairing. The creative tension between anchor and brief is where distinctive work lives. Pick the candidate that produces the most committed result. State the choice and the reason in one line.
3. **Differentiator** — Define one memorable anchor-internal move: a signature interaction, a typographic gesture, a layout motif, or a material treatment. One sentence. Describable. Visible in the rendered output.
4. **System** — Match the chosen anchor's tokens exactly. Picking Swiss means white + sans + grid, not "some flavor of clean."
5. **Implementation** — Outline structure, then build.

Commit fully to one anchor. Hybridising ("Swiss with Brutalist edge") is a category error — each signature excludes the others by construction.

---

## 2. The eight anchors

Each anchor locks specific CSS tokens. Picking the anchor commits to those tokens. If the rendered output drifts outside them, the anchor didn't hold.

### 1. Swiss

**Surface:** Pure white `#FFFFFF` or neutral `#F7F7F8`. **Typography:** Akzidenz-Grotesk, Helvetica Neue, or Söhne — sans display and body, one family. **Accent:** Swiss Red `#E4002B`, International Orange `#FF4F00`, or Yves Klein Blue `#002FA7` — one, used deliberately. **Structure:** visible grid lines or 1 px hairline rules. Left-aligned typography; asymmetric balance. Numerals as composition elements (dates, folio numbers, page markers set in condensed sans).

**Breaks if:** warm paper, serif display, grain texture, or centered typography appears.

### 2. Industrial

**Surface:** Pitch black `#000000` or warm-black `#0B0C0A`. **Typography:** IBM Plex Mono, JetBrains Mono, or Berkeley Mono *throughout* — mono for display too. **Signal color:** one semantic — green `#00E676`, red `#FF3B30`, amber `#FFB800`, or acid lime `#C6FF4A`. **Structure:** flat; 1 px borders do the work shadows would elsewhere. Tabular numerics locked with `font-variant-numeric: tabular-nums`.

**Breaks if:** serif typography, proportional fonts, warm paper, any grain, decorative shadows, or rounded corners appear.

### 3. Brutalist

**Surface:** Pure primary or anti-primary — `#FF0000`, `#0000FF`, `#FFFF00`, `#000000`, `#FFFFFF`. Pick 2–3, compete equally. **Typography:** system fonts only — Times New Roman, Helvetica, Courier, Arial, system-ui. Mix faces deliberately. **Shadows:** hard offset, no blur — `box-shadow: 8px 8px 0 #000`. **Controls:** native browser — unstyled `<button>`, default `<select>`, underlined blue links that stay blue. Margins crushed; type runs edge-to-edge.

**Breaks if:** webfonts, tuned hex beyond pure primaries, soft shadows, rounded corners, or centered layout appear.

### 4. Aurora Maximalism

**Surface:** Dark saturated gradient — `linear-gradient` or `conic-gradient` through violet `#5D34D0` → magenta `#FF006E` → cyan `#00F0FF`, or `#3B82F6 → #A855F7 → #EC4899`. **Typography:** Inter Variable, PP Neue Machina, or Sharp Grotesk for oversized display (15–25 vw). **Texture:** mesh gradient as primary surface feature; neon `text-shadow` glow on accents (`0 0 20px <accent>`). **Motion:** spring-physics orchestration, scroll-linked parallax.

**Breaks if:** flat backgrounds, warm paper, restraint, or hairline rules as primary structure appear.

### 5. Chaotic Maximalism

**Surface:** Clashing palette — pastels *and* neons in the same composition. Hot pink `#FF71CE` + acid yellow `#DFFF00` + cyan `#00FFFF` + any third. **Typography:** mixed faces deliberately colliding — 3+ faces from different registers on the same page. **Texture:** patterns on every surface (squiggles, dots, zigzags, checker — SVG or `repeating-linear-gradient`). Oversized display crashing against busy ground.

**Breaks if:** coherent palette, single typeface, whitespace as structural element, or 60/30/10 dominance appears.

### 6. Retro-Futuristic

**Surface:** Pitch black `#0A0014` or deep navy-black. **Typography:** period-specific — VT323 (CRT), Orbitron (synthwave), Space Mono (cyberpunk), Monoton (Miami-neon), Press Start 2P (arcade), IBM Plex Mono (terminal). **Accent:** neon pair — magenta `#FF006E` + cyan `#00FFFF` (synthwave) or phosphor green `#00FF41` + amber `#FFB000` (terminal). **Texture:** CRT scanlines via `::before` `repeating-linear-gradient` overlay, or chromatic aberration (`text-shadow: 2px 0 #FF0000, -2px 0 #00FFFF`), or both. Glow committed.

**Breaks if:** flatness, modern sans-serifs (Inter, Söhne), paper surfaces, or absence of texture appears.

### 7. Organic

**Surface:** Earth tones — sage `#8B9D83`, clay `#B08B6E`, terracotta `#C66B3D`, ochre `#C08E3A`, moss `#606C38`. When a light surface is needed: sand `#E8DCC7` or oat `#D4B895`. **Never cream `#F0-F8` warm-paper range.** **Typography:** humanist serif (Freight, Caslon, Fraunces — Fraunces is restricted to this anchor only) or warm geometric sans (Greycliff, Epilogue, Recoleta). **Structure:** rounded corners 16–32 px. **Texture:** grain at 1–3 % via SVG feTurbulence. **Motion:** gentle ease 300–500 ms, breathing animations on hero elements.

**Breaks if:** cream backgrounds (warm-tinted `#F0+`), cold greys, pure whites, pure blacks, or hard rectangles appear.

### 8. Lo-Fi

**Surface:** Paper-yellow `#E8E0C0` or `#EDE4CF` — more saturated than cream. **Typography:** mixed system fonts on the same page (Times + Helvetica + Courier colliding deliberately). **Structure:** rotated elements (2–8° off-grid via `transform: rotate`). **Texture:** halftone dot transitions (SVG pattern or `radial-gradient` tile) on imagery; Risograph misregistration (2–4 px RGB channel offset via `text-shadow: 3px 0 #FF006E, -3px 0 #00FFCC`). SVG staple, tape, torn-edge elements.

**Breaks if:** precision, single typeface, smooth motion, rectangles squared to the grid, or cream (the surface is specifically paper-yellow, more saturated) appears.

---

## 3. Output

Every implementation delivers:

- **Stated direction** — A short preamble in a designer's prose before the code, naming: the chosen anchor, the three-candidate deliberation outcome, the differentiator, and the key palette / typefaces / texture choices pulled from the anchor. Written with conviction, not as a checklist.
- **Token fidelity** — The rendered CSS matches the anchor's tokens exactly. If Swiss is chosen, the CSS contains no warm paper, no Fraunces, no grain. If Industrial is chosen, every typeface declared is monospace. Token drift means the anchor didn't hold.
- **Differentiator visible** — The one memorable move is implemented in the rendered output, not merely described.

---

## 4. Before shipping

- **Anchor deliberation** — Did three candidates get named and reasoned about, or did the first instinct win?
- **Token fidelity** — Does every rendered token live inside the anchor's allowed range? If tokens appear that the anchor doesn't allow, the anchor didn't hold.
- **Differentiator visible** — Is the memorable anchor-internal move actually rendered?
- **Hybrid resistance** — Was one anchor held, or did the execution drift into "Swiss with Brutalist edge"?

Intention in every choice. The anchor locks identity at the CSS layer, not just in the preamble.
