# Swiss / International

## Identity

Swiss Style — International Typographic Style — emerged in mid-20th century Switzerland (Müller-Brockmann, Lohse, Bill, Gerstner). Objective clarity, grid systems, sans-serif dominance, asymmetric balance, mathematical proportion. Communication over ornament. Red, black, white, one grid, zero decoration.

The core move: every element has a mathematical reason to sit where it sits. The grid is visible or nearly visible. Typography does most of the work.

## Variants

- **Classical Swiss** — Akzidenz/Helvetica, grid-anchored, red/black/white, poster lineage. Müller-Brockmann territory.
- **Post-Swiss / Modern Grid** — Same discipline, warmer palette, subtle tint, looser but deliberate grid breaks. Spin Studio, Bibliothèque.
- **Hyper-Grid** — Visible grid as design element, numbered systems, rule lines as composition. Experimental Jetset, Wim Crouwel lineage.
- **Typographic Swiss** — Typography nearly the only design element; oversized headline systems, modular type scale. Linear.app aesthetic.
- **Data Swiss** — Swiss discipline applied to data-rich interfaces. Tabular, aligned, colorless except for one signal hue. Stripe documentation, Vercel dashboard.

## Typefaces to Reach For

**Core:** Akzidenz-Grotesk, Helvetica Neue, Neue Haas Grotesk (the original Helvetica redrawn correctly), Univers, Folio.

**Modern Swiss-descendants:** GT America, Söhne, Inter Display, Aperçu, Suisse Int'l, ABC Diatype, Söhne Breit (for display weight).

**Display extrema:** Druk Wide, Söhne Breit, Benton Sans Compressed Black — for poster-scale Swiss energy.

**Monospace for data:** JetBrains Mono, Söhne Mono, ABC Diatype Mono.

Use a single family in 3–5 weights rather than mixing faces. Let weight, case, and scale build the hierarchy.

## Palette Moves

- **High-contrast classical:** Pure white (`#FFFFFF`), pure black (`#000000`), Swiss Red (`#E4002B`) or International Orange (`#FF4F00`) or Yves Klein Blue (`#002FA7`).
- **Muted modern:** Cool grey scale (six steps from `#F7F7F8` to `#0A0A0B`) plus one high-chroma accent.
- **Warmed Swiss:** Soft off-white (`#F5F4F1`), rich near-black (`#0E0D0B`), accent unchanged.
- **Dark mode:** Rich near-black (`#08090B`) + clean near-white (`#F4F4F5`) + accent at full chroma, matched to light mode.

## Composition Moves

- Rigorous 12–16 column grid with visible gutters (or nearly visible — subtle tint difference).
- Asymmetric balance: heavy type-block on one side, whitespace as counterweight. Left-aligned by default.
- Numerical composition: dates, page numbers, issue numbers, section markers become typographic elements in condensed weights.
- Left-aligned always (exceptions must be argued).
- 1 px hairline rules (`border: 1px solid`) as compositional structure, not decoration.
- Overprint: a typographic block overlaps a color field at a mathematically chosen intersection.
- Modular type scale — ratio 1.333 or 1.5 between sizes.

## Motion Flavor

Precise, fast. 150–200 ms. Straight `ease-out` (no spring physics). Hover states shift weight or opacity, nothing jiggles. Grid animates in sequence — columns fill left to right in 40–60 ms staggers. Numerical counters animate with tabular precision (replace digits with `font-variant-numeric: tabular-nums` so width stays locked).

## Depth & Texture

Flat. One elevation level at most (card sits on surface with a 1 px border or a minimal shadow). No gradients other than a possible single-color tint wash. Grain and texture are absent by default — Swiss is pristine.

## Visual References

- **Historic:** Josef Müller-Brockmann, Max Bill, Karl Gerstner, Armin Hofmann, Emil Ruder, Wim Crouwel, Massimo Vignelli.
- **Modern print:** Spin Studio, Bibliothèque, Experimental Jetset, Base Design, Pentagram (select partners).
- **Digital now:** Linear.app, Vercel, Stripe, Arc Browser brand pages, Apollo GraphQL, Raycast, Readwise.
- **Poster lineage:** Swiss concert posters 1955–1975, Der Neue Graphik, Neue Haas publications.
