# Brutalist / Raw

## Values (anti-modernist)

This archetype is **anti-modernist** by construction. Refinement is the failure mode here — system fonts wielded with conviction, hard borders, snap timing, and deliberate misalignment ARE the craft.

**This reference file supersedes the §3 modernist defaults.** Brutalism actively refuses each of them:
- *Hierarchy through 3–5 levels of weight/scale* → Brutalism crushes everything to one weight; "hierarchy" is achieved by raw scale alone (one giant headline, body at default).
- *60/30/10 color dominance* → Brutalism uses pure primaries (`#FF0000`, `#0000FF`, `#FFFF00`, `#00FF00`) at full saturation, often three or more competing equally.
- *Whitespace as structural element* → Brutalism crushes margins; type runs edge-to-edge.
- *Smooth motion via compositor properties* → Brutalism uses 0 ms snap or `steps(1)` — no easing curves, no animation polish.
- *Light-implies-depth shadowing* → Brutalism uses hard offset shadows (`box-shadow: 8px 8px 0 #000`, no blur) that announce themselves as graphic, not material.
- *Asymmetric-balanced composition* → Brutalism uses asymmetry as visible misalignment, often 1–8 degree rotation or pixel-off-grid placement.
- *Custom typefaces from a curated catalog* → Brutalism uses Times New Roman, Courier, Arial, system-ui — shipping system fonts wielded with conviction.

Producing a "polished Brutalism" is a category error — the polish is the failure. Commit to the anti-craft. Read the variants below for the specific moves that constitute it.

## Identity

Brutalism in digital design — raw HTML aesthetic, system defaults wielded as style, aggressive typography, zero ornament. Descends from Brutalist architecture (raw concrete, exposed structure) and the 1990s web (Craigslist, early Geocities, Drudge Report) reclaimed as intentional style. The move is *exposing* rather than hiding.

The core move: show the seams. Default borders, system fonts, visible tables, honest buttons, underlined blue links — wielded with conviction, not apology.

## Variants

- **Classic Brutalist** — Times New Roman or system-ui, underlined blue links, grey backgrounds, visible tables. Looks like a 1996 site, made deliberately now. Craigslist, Hacker News, Berkshire Hathaway.
- **Neo-Brutalist** — Thick black borders (3–6 px), flat saturated primary color blocks, chunky uppercase type, hard drop shadows (`8px 8px 0 #000` with no blur). Gumroad legacy, Figma Community, Are.na, Patterned.io.
- **Typographic Brutalist** — Enormous type crushed against edges, minimal layout, high contrast. Alexey Brodovitch meets 2025 browser.
- **Data Brutalist** — Raw `<table>` elements as design, monospace everywhere, visible columns, exposed data structures. Pudding.cool long-form, NYT interactive features.
- **Web-Native Brutalist** — Embraces browser defaults: native `<select>`, unstyled `<button>`, default form rendering. Zero CSS reset.

## Typefaces to Reach For

**Monospace:** JetBrains Mono, IBM Plex Mono, Space Mono, Berkeley Mono, Fira Code, Courier Prime.

**System defaults used deliberately:** Times New Roman, Courier, Arial Black, system-ui, Georgia, Verdana.

**Chunky display sans:** Helvetica Compressed Black, Druk Wide, Söhne Breit, PP Neue Machina, Akzidenz-Grotesk Super Black.

**Pixel/bitmap for retro-brutalist:** VT323, Silkscreen, Fixedsys, Press Start 2P.

Mixing faces on the same page is a brutalist move — Times + Courier + Arial all in the same composition is legitimate.

## Palette Moves

- **High contrast fundamentals:** `#000000`, `#FFFFFF`, one primary color at full saturation.
- **Web-safe palette aesthetic:** `#FF0000`, `#0000FF`, `#FFFF00`, `#00FF00`, `#FF00FF`. Unapologetic.
- **Classic-brutalist grey:** System chrome `#C0C0C0`, `#E5E5E5`, `#D4D0C8` as backgrounds.
- **Neo-brutalist fields:** Saturated pastel fields (`#FFE77A`, `#A5F0C1`, `#FFB5D8`) with `#000` borders and one neon accent (`#FF006E`, `#00FFAB`).
- **Dark mode:** Pure `#000` + pure `#FFF`, no softening. Brutalist dark refuses tonal compromise.

## Composition Moves

- Margins crushed — type runs edge-to-edge, often with `padding: 0`.
- `<table>` elements as layout grid where appropriate. `border="1"` is honest.
- Visible borders — `border: 3px solid #000` on everything interactive for neo-brutalist.
- Hard drop shadows with zero blur: `box-shadow: 8px 8px 0 #000`, `box-shadow: 12px 12px 0 #FF006E`.
- Intentional misalignment — elements off-grid by a few pixels, or rotated 1–3 degrees.
- Underlined links that stay the web-default blue (`#0000EE`) or a chosen saturated blue.
- Unstyled bullet lists, visible form outlines, native checkboxes.
- Large headline crushed against a screen edge with negative left margin.

## Motion Flavor

Snap or near-zero. Transitions at 0 ms or 50 ms, with `linear` or `steps(1)` timing only. Click equals instant state change. Hover equals color inversion — a hard switch between two states. When motion appears, it's abrupt: a flash, a jolt, a frame-drop flicker. Scroll behaves like browser default — mechanical, jumping to anchors, leaving smoothing and parallax to other archetypes.

## Depth & Texture

Zero conventional depth. Depth comes from hard offset shadows (the signature `box-shadow: Xpx Ypx 0 #000` neo-brutalist move). Texture comes from grain, noise, or deliberate compression artifacts — low-res imagery, pixelated SVG, default browser gradients that look like 2003.

## Visual References

- **Classic:** Craigslist, Hacker News, Drudge Report, Berkshire Hathaway, Motherfucking Website.
- **Neo-brutalist:** Gumroad (legacy), Figma Community, Are.na, Patterned.io, Bloomberg CityLab long-form.
- **Typography-led:** Pudding.cool, Brutalist Websites (the directory), Awwwards brutalist category.
- **Architecture reference:** Paul Rudolph, Alison & Peter Smithson, Marcel Breuer, Lina Bo Bardi. Their built work carries the aesthetic logic.
- **Designers digital:** Stefan Sagmeister (bridge), David Rudnick, Fuzzco (some work), Ben Fry data brutalism.
