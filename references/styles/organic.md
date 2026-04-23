# Organic / Natural

## Identity

Organic / Natural — curved geometry, warm tones, tactile textures, hand-made marks. The opposite of rigid grid. Descends from Art Nouveau curve work, Scandinavian craft, Memphis soft-side, Japanese wabi-sabi, current wellness / craft / farm-to-table brand aesthetic.

The core move: soften the grid. Rounded corners become a whole philosophy. Imperfection becomes a feature. Warmth over coolness across every choice.

## Variants

- **Handcrafted / Artisanal** — Imperfect borders, hand-drawn icons, textured surfaces, warm off-whites, maker-spirit. Our Place, Great Jones, Caraway.
- **Biomorphic** — Organic blob shapes, fluid curves, SVG morphing, asymmetric soft geometry. Linear hero blobs, Framer blob generators, ibelick.com components.
- **Scandinavian Craft** — Muted earth tones, humanist serifs, pottery-adjacent warmth, functional calm. HAY, Ferm Living, Muuto, Skagerak.
- **Wellness / Spa** — Soft gradients (sage to cream), breathing motion, round corners, no hard edges. Headspace, Calm, Peloton (select), Goop wellness sections.
- **Painterly / Gallery** — Painterly textures, brush strokes, watercolor washes, collage feeling. Small independent gallery sites, artist portfolios.
- **Farm-to-Table / Natural Food** — Kraft-paper textures, hand-lettered labels, warm neutrals with one produce-inspired accent. Blue Hill, Salt & Straw, many craft food brands.

## Typefaces to Reach For

**Humanist serifs:** Freight Text, Freight Display, Caslon, Meridien, Sabon, Kepler, Sentinel, Adelle, Caponi.

**Soft sans (humanist, rounded):** Greycliff, Epilogue, Archivo, Manrope, Nunito (sparingly), Söhne Breit (for quieter moments), Recoleta (rounded serif-adjacent).

**Hand-drawn accent faces:** Caveat, Homemade Apple, Permanent Marker, Kalam — reserved for annotations, signatures, and short notes.

**Warm display:** Recoleta, Playfair (in its soft cuts), Fraunces (variable — expressive), Domaine.

## Palette Moves

- **Earth tones as core:** clay (`#B08B6E`), terracotta (`#C66B3D`), sage (`#8B9D83`), ochre (`#C08E3A`), moss (`#606C38`), oat (`#D4B895`), cream (`#F3E9D2`).
- **Warm off-whites:** ivory (`#F8F4EC`), bone (`#F2EDE0`), parchment (`#EDE4D1`), sand (`#E8DCC7`).
- **Desaturated accents:** muted teal (`#5B8A8A`), dusty rose (`#C9A9A6`), faded gold (`#B89A6C`), sun-bleached red (`#C1584E`).
- **Dark mode:** warm earth-black (`#231E16`) + cream text (`#EDE4D1`). Accents stay the same — organic dark mode is sunset, not night.

## Composition Moves

- **Rounded corners everywhere** — 16–32 px is the baseline; heroes can go 48–64 px on large surfaces.
- **Blob shapes** — SVG blobs for hero backgrounds, `border-radius` with variance (`border-radius: 62% 38% 54% 46% / 45% 55% 45% 55%`) for organic quadrilaterals.
- **Asymmetric layouts** with organic flow — content follows a curve, not a grid line.
- **Grain overlays** on every surface (1–3% opacity noise via SVG `<feTurbulence>` or a tiled PNG).
- **Paper-textured backgrounds** — subtle noise + warm tint simulating parchment, linen, or kraft.
- **Hand-drawn divider marks** instead of rules — SVG squiggle lines, pencil-drawn asterisks, wavy underlines.
- **Circular image frames**, soft-cornered photography, lifestyle imagery with warm tone grading.
- **Letterpress-inspired depth** — slight inset shadow on type suggesting physical impression on paper.

## Motion Flavor

Soft and gentle. 300–500 ms eases. Springs with gentle damping (Framer Motion `{ type: 'spring', stiffness: 100, damping: 20 }`). Breathing animations — subtle scale oscillation (0.98 ↔ 1.02 on a 4-second loop) on hero elements. Curved path motion — Bezier curves for position tweens. Fluid morphs between states feel continuous from one to the next. Reveals combine opacity and translate gently.

## Depth & Texture

Tactile. Grain is near-universal (a `<feTurbulence>` noise layer at low opacity on the base surface). Paper textures on backgrounds. Soft diffuse shadows — `box-shadow: 0 12px 32px rgba(100, 80, 60, 0.12)` in a warm-tinted rgba to match the palette. Layered shadows for blob hero elements. Watercolor washes via radial gradients with low opacity stops. Letterpress-style inset type where appropriate.

## Visual References

- **Digital:** Aesop (bridges organic/minimalist), Our Place (homesick.com), Great Jones, Caraway, Oatly, The Sill, Milk Bar, Loisa, Haus.
- **Scandinavian craft:** HAY, Ferm Living, Muuto, Skagerak, &Tradition, Frama.
- **Wellness:** Headspace, Calm, Peloton (sections), Goop sections, Apartamento magazine, The School of Life.
- **Designers:** Alvar Aalto (product + brand lineage), Enzo Mari, Nendo (minimalist-adjacent), Kenya Hara (wabi-sabi-adjacent).
- **Physical:** Japanese pottery (raku, shino glazes), Scandinavian ceramics, hand-letterpress books, Apartamento apartment photography.
