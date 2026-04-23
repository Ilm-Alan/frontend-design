# Minimalist / Refined

## Identity

Minimalism as craft — restraint, not emptiness. Every element has earned its place. Ample whitespace, micro-contrast, meticulous spacing, hairline dividers, precise optical alignment. Descends from Dieter Rams ("Less, but better"), Japanese wabi-sabi, John Pawson architecture, Apple's design lineage under Ive.

The core move: remove until removing any more would break it, then polish what remains.

## Variants

- **Nordic Minimalist** — Warm off-white, soft geometric serifs or humanist sans, pale accents, considered imperfection. Norse Projects, Acne Studios, HAY.
- **Japanese Minimalist** — Asymmetric void, single strong mark, type as poetry, dramatic whitespace ratios. Muji, Kenya Hara, Nendo, Issey Miyake brand.
- **Tech Minimalist** — Apple-lineage: geometric sans, subtle elevation, systems-driven spacing, generous line-height. Apple.com, Linear, Arc, Notion (restrained mode), Things 3.
- **Luxury Minimalist** — Single serif face, expanded letter-spacing in caps, sparse gold or silver accent, dramatic negative space. Hermès, Aesop, Le Labo, Goop (select sections).
- **Swiss-adjacent Minimalist** — Minimalism with grid discipline; less asymmetric void than Japanese, more rule-bound. Braun product pages, Teenage Engineering.

## Typefaces to Reach For

**Sans:** Söhne, GT America, Untitled Sans, Aperçu, SuisseWorks, SF Pro (used with restraint), Söhne Schmal for captions.

**Serif:** Domaine Text, Freight Text, Tiempos Text, Hoefler Text, SuisseWorks (its serif counterpart), Ogg (for subtly expressive minimalism).

**A single family used across 4–5 weights is often enough.** Mixing faces is discouraged except for deliberate serif display + sans body (or the reverse).

**Monospace:** Berkeley Mono, Söhne Mono — for data or selective accent only.

## Palette Moves

- **Near-monochrome core:** Off-white + near-black + one desaturated accent.
- **Warm whites preferred** over cold: `#FAF7F2`, `#F4F1EC`, `#F8F5F0`. Cold whites read clinical; warm whites read considered.
- **Deep near-black body:** `#0F0E0C`, `#1A1816`. Reserve full `#000000` for the luxury-minimalist variant.
- **Single accent, muted:** sage (`#8B9D83`), clay (`#B08B6E`), slate (`#546272`), oxblood (`#6B2C2C`), faded gold (`#B89A6C`).
- **Dark mode:** Rich warm black (`#0E0C09`) + paper white (`#EDE6D8`), not grey-on-grey. Accent holds or shifts slightly warmer.

## Composition Moves

- Massive whitespace — 30–50% of the visible area. On hero screens, 60%+ empty is acceptable.
- 1 px hairline dividers via `border-top: 1px solid var(--color-border)` instead of bordered boxes.
- Optical alignment — center text blocks align to the optical center of the letterform, not the geometric edge. Nudge by 1–3 px where needed.
- Dramatic scale ratios — 6:1 or higher between display and body. The display is the event.
- Single-column hero moments on wide screens. Widescreen is not an invitation to fill.
- Generous line-height on body (1.65–1.85). Breath matters.
- Typography does the ornament — small caps, old-style figures, subtle italic distinction.

## Motion Flavor

Restrained and refined. 200–400 ms eases. Ease-out for entrances (`cubic-bezier(0.16, 1, 0.3, 1)` — the gentle snap used by Linear and Apple). Subtle transforms: scale from 0.98 to 1, opacity 0 to 1, translate 8–12px. Scroll-linked animation reveals content with restraint — one element at a time, with deliberate pacing between each.

## Depth & Texture

One-to-two elevation levels maximum. Shadows are soft and small — `box-shadow: 0 1px 2px rgba(0,0,0,0.04), 0 4px 12px rgba(0,0,0,0.04)`. Glass effects are rare; when used, very light blur (6–10 px) with high opacity backgrounds. Grain at 1–2% for warmth. No mesh gradients, no bold textures — the archetype's whole point is fewer visible moves.

## Visual References

- **Digital:** Apple.com, Aesop.com, Muji.com, Linear.app, Arc Browser, Things 3 app, Notion, Krea.ai, Acme.studio.
- **Print / brand:** Muji, Aesop, Norse Projects, Acne Studios, MNML, Hermès select pages.
- **Designers:** Dieter Rams, Naoto Fukasawa, Kenya Hara, John Pawson, Jasper Morrison, Jony Ive (early Apple). For digital: Rauno Freiberg, Shawn Park, Jordan Singer.
- **Physical reference:** Braun products 1960–1980, Muji notebooks and home goods, Teenage Engineering OP-1.
