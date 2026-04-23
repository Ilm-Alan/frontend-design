# Retro-Futuristic

## Identity

Nostalgia for futures imagined in the past — 1980s cyberpunk, synthwave, vaporwave, Y2K, early-digital. Neon on dark, CRT artifacts, glow, scanlines, pixelation as aesthetic choice. The lineage: Blade Runner, Akira, Tron, Japanese VHS covers, early Macintosh HyperCard, Windows 95 chrome reinterpreted.

The core move: choose an era's imagined future and commit to its visual grammar. This archetype fails when it dabbles in several futurisms at once.

## Variants

- **Synthwave** — Sunset gradients (pink → purple → orange), chrome lettering, wireframe horizons, neon grid floor. Miami Vice meets The Midnight album covers.
- **Cyberpunk** — Neon green/magenta on pitch black, glitch, dense technical typography, monospace overload, Japanese katakana as ornament. Blade Runner, Ghost in the Shell, Cyberpunk 2077 UI.
- **Vaporwave** — Pastel pink + cyan, Greek sculpture motifs, Windows 95 UI chrome, Japanese katakana, mall ambiance. Floral Shoppe, early 2010s Tumblr aesthetic.
- **Y2K** — Chrome, bubble text, translucent plastic, Frutiger Aero, glossy orbs, iMac G3 color palette. 1999–2003 web and product design.
- **CRT / Terminal** — Phosphor green on pure black, scanlines, amber monochrome for variant, Commodore-era pixel fonts. Fallout terminals, The Matrix code rain.
- **Atompunk / Space Age** — Mid-century futurism, chrome + orange + teal, Saul Bass title sequence energy, Jetsons optimism. Eero Aarnio, Verner Panton product design.

## Typefaces to Reach For

**Pixel / bitmap:** VT323, Silkscreen, Press Start 2P, Pixelify Sans, Fixedsys Excelsior, DEC Terminal, Pixeloid Sans.

**Display (retro-futurist sans):** PP Neue Machina, Blanka, Orbitron (earnestly, as it's right for the era), Unica One, Druk Wide, Monument Extended, CA Silver.

**Monospace (terminal):** Space Mono, Courier Prime, Major Mono Display, IBM Plex Mono, Victor Mono.

**Geometric sans (atompunk):** Eurostile, Futura, Avenir Next, Neue Haas Unica — for mid-century futurism.

**Chrome / custom lettering:** SVG-based custom letterforms with gradient fills are often the signature — no font captures chrome like an actual metallic gradient on outlined type.

## Palette Moves

- **Cyberpunk:** Neon on deep — `#FF006E` magenta, `#3A86FF` electric blue, `#06FFA5` mint green on `#0A0014` or `#1A0033` near-black.
- **Synthwave:** Gradient pink (`#FF006E`) → purple (`#8338EC`) → orange (`#FB5607`), over a dark navy (`#0F0E17`) base with a horizon line.
- **Terminal green:** `#00FF41` phosphor on `#0D0208`. Or amber variant: `#FFB000` on `#0F0804`.
- **Y2K:** Translucent blues (`#AFDCEC`) + chrome silvers (`#C0C0C0`) + hot pink (`#FF10F0`) + black. iMac Bondi Blue (`#5BB5C9`).
- **Vaporwave:** `#FF71CE` pastel pink + `#01CDFE` cyan + `#05FFA1` mint + `#B967FF` lavender on `#FCEBF8` cream or deep navy.
- **Atompunk:** Chrome silver + orange (`#FF6B35`) + teal (`#00A896`) + cream + deep black.

Chromatic aberration (RGB channel split) as texture: slight `text-shadow: 2px 0 #FF0000, -2px 0 #00FFFF` on hero type.

## Composition Moves

- Wireframe grids as background — perspective floor with horizon line (SVG or CSS transform), synthwave style.
- CRT scanlines via `::before` overlay: `repeating-linear-gradient(0deg, transparent 0, transparent 2px, rgba(0,0,0,0.15) 2px, rgba(0,0,0,0.15) 4px)`.
- Glitch effects — keyframes that skew, offset, hue-rotate on hover or at intervals (`transform: translate(2px, 0) skew(1deg); filter: hue-rotate(90deg)`).
- Oversized chrome lettering — SVG text with `linearGradient` fill simulating chrome, outlined in a darker stroke.
- Terminal windows as layout containers — titlebar + window chrome + monospaced content. Commits hard to the metaphor.
- ASCII art as compositional elements — headers, dividers, logo marks built in characters.
- Barcode, QR code, fake-technical graphics as ornament.
- Japanese katakana (カタカナ) alongside Latin text for cyberpunk authenticity.

## Motion Flavor

- **Glitch:** Micro-jumps, hue shifts, RGB splits on hover and at intervals.
- **Neon pulse:** Slow 2–3 second brightness cycle on accent elements (`text-shadow` opacity animation).
- **Typewriter reveals:** Letter-by-letter text appearance for terminal/CRT styles. Use `steps()` timing for authenticity.
- **Scanline drift:** Slow vertical animation of the scanline overlay (20–30 second loops).
- **Shake on hover:** Small random 2–3 px displacement for cyberpunk interactive elements.
- **Boot sequence:** Page load treated as a terminal boot — text appears line by line, cursor blinks between.

## Depth & Texture

Texture-heavy. Noise, scanlines, chromatic aberration, film grain, VHS tracking lines all live here. Depth comes from layered neon glow (`text-shadow: 0 0 10px #FF006E, 0 0 20px #FF006E, 0 0 40px #FF006E`) rather than box-shadows. Glass effects stylized to feel like plastic or plexiglass (Y2K) rather than Apple-glass. Chrome gradients on outlined shapes.

## Visual References

- **Films/games:** Blade Runner (1982 & 2049), Akira, Tron, Hackers (1995), The Matrix, Cyberpunk 2077, Outer Wilds UI, Returnal UI, Kung Fury.
- **Music / album art:** The Midnight, FM-84, Perturbator, Carpenter Brut, Floral Shoppe, Daft Punk.
- **Digital now:** The Verge "Re: Web" redesign (2022), Spotify Wrapped (select years), Sorry I Don't Dance, Nomad List (retro-adjacent), Dribbble cyberpunk explorations.
- **Lineage designers:** Saul Bass (atompunk roots), Syd Mead (concept art), Paul Rand (retro-modern), Japanese VHS cover artists of the 1980s.
- **Physical:** Braun + early Sony product design (atompunk), 1980s arcade cabinets, CRT monitors, Commodore 64 boot screens.
