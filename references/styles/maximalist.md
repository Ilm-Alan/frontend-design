# Maximalist / Expressive

## Values (varies by sub-mode — pick before committing)

This archetype contains **two opposite value systems**. Decide which mode the brief calls for *before* picking moves:

- **Modernist Maximalism** (Aurora / Gradient, Liquid Glass, 3D / Hyperrealism) — *ambitious but coherent*. The §3 modernist defaults apply: token systems, color discipline, smooth motion, dramatic-but-resolved hierarchy. The "more" is layered with intention; every gradient stop is tuned, every motion curve is custom. Stripe, Linear, Vercel, Rauno Freiberg territory.

- **Anti-modernist Maximalism** (Memphis Revival, Vibrant Block, chaotic-pattern) — *productive chaos*. The §3 modernist defaults are reference points to react against. Clashing pastels + neons, pattern-heavy surfaces, deliberate visual noise, oversized display crashing against busy backgrounds. Memphis Group (Sottsass), Mailchimp illustrations, Duolingo marketing, riot-color Web3.

These are not the same archetype with different palettes — they have **opposite values**. A Memphis-leaning brief and a Stripe-Aurora-leaning brief require entirely different commitment patterns. Pick the sub-mode in §1.2 (Aesthetic Direction); name it in the preamble alongside the archetype label.

If the chosen sub-mode is anti-modernist Maximalism, this reference file supersedes the §3 modernist defaults — chaotic Maximalism shares Brutalism's and Lo-Fi's anti-craft stance, just expressed through abundance rather than reduction.

## Identity

Maximalism — visual abundance, layered composition, saturated color, ambitious motion. More is more, disciplined. Descends from Italian Memphis (1980s), Japanese graphic design of the 80s–90s, current creative studio / Web3 / hero-section-as-spectacle aesthetic.

This archetype absorbs several contemporary sub-styles: Aurora UI (gradient-forward), Liquid Glass (morphing chromatic), Vibrant Block (saturated geometric), and 3D / Hyperrealism (Three.js-powered). They share the DNA: abundance, saturation, motion, layered depth.

The core move: layer intentionally. Abundance without composition reads as chaos; maximalism works when every layer earns its place and the whole has a conductor.

## Variants

- **Aurora / Gradient Maximalist** — Mesh gradients, iridescent surfaces, long smooth color blends, glow. Stripe hero sections, Linear hero, Framer marketing, Vercel OG.
- **Liquid Glass / Morphing** — Chromatic aberration, SVG morph animations, fluid blurs, oil-slick palettes, holographic surfaces. Apple VisionOS aesthetic, emerging iOS 26 style language.
- **Vibrant Block** — Saturated color blocks, chunky geometric shapes, bold typography at 80px+, scroll-snapped sections, playful primaries. Klarna, Revolut (select moments), Duolingo marketing.
- **3D / Hyperrealistic** — Three.js / React Three Fiber integration, WebGL surfaces, realistic lighting, parallax layers, object-centric hero. Arc browser 3D cursor, Rauno.me, Ben Borgers, Vercel OG template site.
- **Memphis Revival** — Pattern-heavy (squiggles, dots, zigzags, grids), clashing pastels + neons, playful chaos, intentional retro. Mailchimp illustrations, Duolingo, Slack emoji aesthetic.

## Typefaces to Reach For

**Display (expressive serif):** PP Editorial New, Migra, Reckless Neue, Eiko, Tobias, F37 Ginger, Domaine Display — the display does the heavy lifting; body stays restrained.

**Display (expressive sans):** PP Neue Machina, PP Right Grotesk, Sharp Grotesk, Söhne Breit, Moranga, Druk Wide.

**Variable type** for dramatic weight play: Söhne Variable, Inter Variable, Sharp Grotesk Variable, Name Sans.

**Body:** Söhne, GT America, Inter — restrained so display can scream. Body is the conductor letting the soloist shine.

Sizes run 15–25 vw for hero display. Tracked tight (`letter-spacing: -0.03em`) at those sizes.

## Palette Moves

- **Saturated primary triads:** electric blue + hot pink + acid yellow (`#0066FF`, `#FF00AA`, `#FFEE00`); deep violet + coral + mint (`#5D34D0`, `#FF6B6B`, `#4ECDC4`).
- **Aurora gradient pairings:** blue → purple → pink (`#3B82F6 → #A855F7 → #EC4899`), orange → red → magenta (`#F59E0B → #EF4444 → #D946EF`), teal → lime → yellow.
- **Iridescent / holographic:** oil-slick palettes that shift hue across the surface. Implemented with `conic-gradient` or multi-stop `linear-gradient`, blend-mode `overlay` or `screen`.
- **Dark maximalism:** Deep navy (`#0A0A2E`) or pure black base with neon accents pulsing through.
- **Six-color palettes** instead of three — use them with 60/30/10 discipline so abundance doesn't collapse into noise.
- **Dark mode:** Often the primary mode for maximalist web; light mode takes more tuning since saturated color needs deeper fields to glow against.

## Composition Moves

- Overlapping layers: type on imagery on gradient, each with its own z-index and blend-mode.
- Asymmetric grid breaks on every screen — nothing centered, nothing predictable.
- Full-bleed sections with dramatic color shifts between them (section 1 deep violet; section 2 acid yellow; section 3 noir with one accent).
- Z-stack composition with intentional depth — foreground text, midground shape, background gradient, all moving at different rates on scroll.
- Oversized display type (15–25 vw) clipped or bleeding off edges.
- Mixed media: 3D object + flat type + photography + gradient mesh on the same surface.
- Scroll-triggered color shifts — the entire page background animates from one gradient to another as you scroll.

## Motion Flavor

Ambitious and orchestrated. Spring physics (Framer Motion or spring-based CSS). Scroll-linked parallax. Color transitions on scroll. 400–800 ms for orchestrated reveals. Cursor-driven effects: magnetic buttons, cursor-trailing gradient, cursor-driven mesh distortion. Three.js / React Three Fiber / GSAP / Framer Motion territory.

Stagger entrances with rhythm — 60–80 ms per item for hero-section reveals (longer than minimalist's 30–50 ms because the motion is more theatrical).

## Depth & Texture

Layered aggressively. Multiple elevation levels, each with its own shadow character. Glassmorphism heavy: `backdrop-filter: blur(20px) saturate(1.5)` on floating surfaces. Grain overlays at 3–5% for warmth. Mesh gradients (multi-stop `conic-gradient` or Rauno-style SVG mesh). Noise textures via SVG `<feTurbulence>`. Chromatic aberration on hover states for premium moments.

## Visual References

- **Digital (now):** Stripe, Linear (hero), Arc Browser, Vercel, Framer marketing, Rauno.me, emilkowal.ski, aarver.xyz, ibelick.com, Ben Borgers (benborgers.com).
- **Studios:** Tendril, Active Theory, Immersive Garden, Locomotive, Hoverstate, Humbleteam, Ueno (legacy).
- **Brands:** Klarna, Revolut marketing, Duolingo, Glossier (playful variant), Notion marketing (restrained variant).
- **Lineage:** Memphis Group (Ettore Sottsass), Japanese graphic design 1980s (Tadanori Yokoo, Ikko Tanaka), Peter Saville (maximalist period), David Carson.
- **3D artists / tools:** Three.js examples, Spline, React Three Fiber showcases, Vercel OG playground.
