# Archetype values

Each archetype carries values that shape what counts as commitment. Modernist values demand refinement, coherence, and intention. Anti-modernist values demand roughness, productive contradiction, and deliberate mess. Hybrid values demand commitment to a specific frame (a particular era's imagined future, warmth-as-discipline) rather than the generic version of either pole.

The §3 modernist craft rules in `SKILL.md` apply by default. For anti-modernist archetypes, the per-archetype entries below override those rules.

---

## Modernist archetypes

**Editorial, Swiss, Minimalist, Industrial, Art Deco** — and the modernist sub-modes of Maximalism (Aurora / Gradient, Liquid Glass, 3D / Hyperrealism).

Commit to refined craft:

- Specific named typefaces (not system fallbacks)
- A palette derived from `palettes.md` with semantic tokens, or named hex values tuned with the tuning stated
- Smooth motion via compositor properties (transform, opacity)
- Hierarchy through 3–5 levels of weight, scale, case, and tracking
- 60/30/10 color dominance
- Texture stays flat unless the archetype explicitly names a texture move (paper grain at 2–4% for Editorial, scanlines for Retro-Futuristic, etc.)

Industrial and Swiss treat flatness as identity — no grain, no glass, no shadows except hairline borders.

---

## Anti-modernist archetypes

**Brutalist, Lo-Fi, chaotic Maximalism (Memphis Revival, Vibrant Block).**

These archetypes refuse the modernist defaults. Refinement is the failure mode. Polish reads as betrayal of the brief.

### Brutalist / Raw

Anti-decoration, exposed structure, system defaults wielded as deliberate style.

Commitments:

- System fonts (Times New Roman, Helvetica, Courier, Arial, system-ui) used deliberately. **No webfonts.**
- Pure primary colors at full saturation (`#FF0000`, `#0000FF`, `#FFFF00`, `#00FF00`) — three or more competing equally is fine.
- Type runs edge-to-edge; margins crushed.
- Hard offset shadows: `box-shadow: 8px 8px 0 #000`, no blur. The shadow announces itself as graphic, not material.
- 0 ms snap or `steps(1)` motion. No easing curves.
- Visible misalignment (1–8 degree rotation, off-grid by pixels).
- Default browser controls visible: native `<select>`, unstyled `<button>`, underlined blue links that stay blue.

Refusing:

- Custom typefaces from a curated catalog
- 60/30/10 dominance
- Whitespace as structural element
- Smooth motion via compositor properties
- Light-implies-depth shadowing
- Hierarchy through tuned weight/scale ladders

A "polished Brutalism" is a category error — the polish is the failure.

### Lo-Fi / Zine

Deliberate clash, photocopier roughness, productive imperfection.

Commitments:

- Mixed typefaces selected for collision (Helvetica + Times + Courier on the same page; the clash is the move).
- Risograph two-color overlays with deliberate misregistration (2–4 px offset between plates).
- "Bad" combinations through conviction (mustard on lilac, brown on purple).
- Snap, flicker, jolt motion. Page-tear reveals.
- Staple marks, torn paper edges (`clip-path: polygon(...)`), visible tape.
- Halftone dot transitions on photography.
- Rotated elements (2–8 degrees off-grid as if taped on).
- Photocopier grain (heavy, not subtle).

Refusing:

- Coherent typeface pairings
- 60/30/10 color dominance
- Whitespace as structural element
- Smooth motion
- Hairline rules and refined dividers
- Optical type alignment

A "polished Lo-Fi" is a category error — the imperfection is the entire point.

### Chaotic Maximalism (Memphis Revival, Vibrant Block sub-modes)

Productive chaos through abundance.

Commitments:

- Pattern-heavy surfaces (squiggles, dots, zigzags, grids).
- Clashing pastels and neons in the same palette.
- Oversized display (15–25 vw) crashing against busy backgrounds.
- Saturated triads (electric blue + hot pink + acid yellow).

This sub-mode shares Brutalism's and Lo-Fi's anti-craft stance, just expressed through *abundance* rather than *reduction*. **Distinct from modernist Maximalism** (Aurora, Liquid Glass, 3D / Hyperrealism), which is *ambitious but coherent* and follows the §3 modernist defaults. Pick the sub-mode in §1.2 (Aesthetic Direction); name it in the preamble alongside the archetype label.

---

## Hybrid archetypes

### Retro-Futuristic (nostalgic precision)

Commit to one era's imagined future with conviction; refuse generic "retro." Period-appropriate typefaces (VT323 and IBM Plex Mono for terminal/CRT; Orbitron, Space Mono, Monoton for synthwave; Eurostile, Futura for atompunk; chrome SVG lettering for outrun). Deep dark base + saturated period-correct accents.

The §3 modernist defaults mostly apply, but **texture is heavy and committed** (CRT scanlines, neon glow via layered `text-shadow`, chromatic aberration, perspective wireframe grids) rather than flat. The archetype's identity lives in the texture; flatness would betray it.

### Organic (warmth-as-discipline)

Soft geometry, earthy palette, tactile texture, hand-drawn marks. **Calm is the success mode; over-styling is the failure.** The §3 defaults apply with warmer execution: warm off-whites instead of cold ones, rounded corners (16–32 px), grain at 1–3% on every surface, soft 300–500 ms eases with gentle springs (Framer Motion `{ stiffness: 100, damping: 20 }`), breathing animations on hero elements.

Anti-modernist sister archetypes (Brutalist, Lo-Fi) reject Organic's gentleness; Editorial and Minimalist sit closest in spirit (refinement through restraint).
