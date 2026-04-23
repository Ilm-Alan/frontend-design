# Lo-Fi / Zine

## Values (anti-modernist)

This archetype is **anti-modernist** by construction. Coherence is the failure mode here — deliberate clash, mixed typefaces on the same page, torn edges, photocopier artifacts ARE the craft.

**This reference file supersedes the §3 modernist defaults.** Lo-Fi actively refuses each of them:
- *Pair a distinctive display face with a body face* → Lo-Fi mixes Helvetica + Times + Courier on the same page; the clash is the move.
- *60/30/10 color dominance* → Lo-Fi uses Risograph two-color overlays with deliberate misregistration, intentionally "bad" combinations (mustard on lilac, brown on purple) that work through conviction.
- *Whitespace as structural element* → Lo-Fi fills corners with annotations, stamps, taped photos, hand-drawn arrows.
- *Smooth motion via compositor properties* → Lo-Fi uses snap, flicker, jolt, page-tear reveals; no easing curves.
- *Hairline rules and refined dividers* → Lo-Fi uses staple marks, torn paper edges, visible tape, halftone dot transitions.
- *Light-implies-depth shadowing* → Lo-Fi uses harsh ink-bleed shadows or no depth at all; flatness is paper, not screen.
- *Optical type alignment* → Lo-Fi rotates elements 2–8 degrees off-grid as if taped on; precision is the enemy.

Producing a "polished Lo-Fi" is a category error — the imperfection is the entire point. Commit to the deliberate mess. Read the variants below for the specific moves that constitute it.

## Identity

Lo-Fi / Zine — rough textures, photocopier artifacts, collage, deliberate imperfection, riot grrrl zine energy. Descends from punk flyers, 1970s mimeograph, DIY pamphlet culture, cut-and-paste album art, Linder Sterling collages, Raymond Pettibon, David Carson's Ray Gun.

The core move: commit to making it look hand-made, photocopied, xeroxed, or Riso-printed. Digital precision is the enemy; imperfection is the voice.

## Variants

- **Classic Zine** — Photocopier grain, torn paper edges, staple marks, xerox halftone, mixed type cut from magazines. 1990s riot grrrl zines.
- **Punk Flyer** — Collage type cut from newspapers, high-contrast photocopy, aggressive composition, rotated elements. Search & Destroy, Sniffin' Glue, Maximum Rocknroll.
- **Sticker / Patch** — Layered sticker graphics, distressed edges, DIY aesthetic, skate-culture bleed. Thrasher, Palace Skateboards, street-art-adjacent.
- **Newsprint / Tabloid** — Dot halftone, cheap ink bleed, columnar layout, tabloid-sensational headlines. The Onion print era, Village Voice.
- **Mixtape / Cassette** — Handwritten labels, marker text, smudged imperfection, personal-mix-tape intimacy. Lo-fi hip-hop cover art, bandcamp small-label.
- **Risograph** — Bold two-color prints (pink + blue, yellow + green), misregistered overlays as design, limited palette as constraint. Current indie publishing, small-press zines.

## Typefaces to Reach For

**Mixed (intentionally):** Helvetica + Times + Courier on the same page. The clash is the move.

**Typewriter:** Courier Prime, American Typewriter, VT323, Speidel Olympia.

**Distressed / beat-up:** PP Mondwest, PP Right Grotesk in its rough cuts, Druk used beat-up, Monument Extended stressed, free fonts with wear.

**Hand-written:** Permanent Marker, Caveat, Rock Salt, Homemade Apple, Shadows Into Light — for accent, not body.

**Photocopy-damaged fonts:** any face rendered onto a noise-filter overlay reads as xeroxed. Or custom-distress a clean font via SVG filter effects.

**Newsprint serif:** Old Standard TT, New York, specific newspaper fonts where available.

## Palette Moves

- **Newsprint:** Cream / yellowed paper (`#E8E2D1`, `#EDE4CF`) + black ink + one cheap-ink spot (blotchy red `#D63535`, or blue `#2A4BBE`). Ink bleeds are a feature.
- **High-contrast two-color risograph:** hot pink (`#FF0066`) + royal blue (`#0033CC`); chartreuse (`#DFFF00`) + magenta (`#CC0099`); red (`#FF3333`) + teal (`#00A0A0`). Misregistration (~4 px offset) between the two layers.
- **Xerox toner black on paper-yellow:** `#1A1A1A` on `#F5F0DC` with paper grain throughout.
- **Punk flyer:** Pure `#000000` + pure `#FFFFFF` + one shock neon (acid green `#CCFF00`, hot pink `#FF0099`).
- **Mixtape:** handwritten inks on cream — navy ballpoint, red Sharpie, black marker, on `#F5F0E1` paper.
- **Intentionally "bad" combos** that work through conviction — mustard on lilac, brown on purple, anything that feels xeroxed-together.

## Composition Moves

- **Rotated elements** — text blocks and images at 2–8 degree angles, as if taped on.
- **Torn paper edges** — SVG `<mask>` with irregular torn shape, or `clip-path: polygon()` with jagged coordinates.
- **Halftone photography overlays** — dot pattern via SVG or CSS `radial-gradient` tiling, reducing photos to black-and-white dots.
- **Collage composition** — overlapping layers at different scales, some oversized, some tiny, with tape or staple graphics between them.
- **Visible tape, staple, pin marks** — small SVG elements placed as if fixing collage pieces in place.
- **Misregistered color prints** — slight RGB offset on images (chromatic aberration as print artifact, not cyberpunk glow).
- **Handwritten annotation overlays** — scrawls, arrows, circled words on top of typeset content, like a printed draft with notes.
- **Column layouts with bad kerning intentional** — justified text with huge gaps where a newspaper column broke poorly.
- **Stamps, seals, rubber-stamp marks** as decorative authority.

## Motion Flavor

Snap / flicker / jolt. Transitions at 0–80 ms with `steps(1)` for stepped motion. Shake on hover — small random 2–3 px displacement. Page-flip or paper-tear reveals. Analog-feeling imperfection: no smooth curves, no spring physics. Boot-up flicker effect for initial reveal. Cut between states rather than transition (one frame → different frame, hard cut).

Print-press effect for color changes: one color layer shifts independently of the other (the Riso misregister as animation).

## Depth & Texture

Texture is the archetype. Paper grain everywhere — `<feTurbulence>` noise layers, or tiled PNG of scanned paper. Halftone dots for images and some flat surfaces. Toner streaks (thin vertical lines of slightly lighter color, simulating xerox drum wear). Coffee stains, ring marks, creases, folds — all period-appropriate scans overlaid. Drop shadows are harsh and printed — `box-shadow: 4px 4px 0 #000`, or a smudged ink-bleed version.

Chromatic aberration as print misregistration (2–4 px offset) rather than cyberpunk glow — same technique, different aesthetic register.

## Visual References

- **Zine history:** Search & Destroy, Sniffin' Glue, Maximum Rocknroll, Riot Grrrl (various), Bust, Bikini Kill zine, ProfanExistence, Cometbus.
- **Album art / music:** Sex Pistols (Jamie Reid), Joy Division (Peter Saville's rougher work), Crass, early Sub Pop, K Records, Olympia scene.
- **Photocopy / xerox artists:** Linder Sterling, Raymond Pettibon, Jamie Reid, Barbara Kruger (bridge), Winston Smith.
- **Modern lo-fi digital:** Are.na aesthetic, Recess Magazine, It's Nice That features, Dina Sans's essay layouts, Riso printshops (Hato Press, Colour Code).
- **Film:** Ghost World, Slacker, How to Blow Up a Pipeline, documentaries about DIY punk scenes.
- **Designers:** David Carson (Ray Gun era, the bridge to digital), Ed Fella, Art Chantry, Lou Beach, Stefan Sagmeister (some work), April Greiman's early computer-made zines.
