# Industrial / Utilitarian

## Identity

Industrial / Utilitarian — function exposed, data-first, monochrome, dense information layouts, instrument-panel energy. Descends from military HUDs, aerospace instrumentation, scientific apparatus, Bloomberg Terminal, Bauhaus workshop, Dieter Rams engineering aesthetics.

The core move: every pixel carries information. Decoration is replaced by data, labels, and precise hierarchy. The interface is a tool, and looks like one.

## Variants

- **Engineering / Technical** — Dense data, monospace typography, blueprint aesthetic, grid rulers visible, schematic feel. GitHub (legacy), Stripe documentation, engineering dashboards.
- **Dashboard / Observability** — Chart-heavy, color-coded status, multi-panel layouts, real-time data feel. Grafana, Datadog, Linear's insights, Vercel dashboard.
- **Terminal / CLI** — Monospace everywhere, ASCII tables, command-line aesthetic moved to GUI, green-on-black or amber-on-black options. Warp, Wezterm marketing, Kitty terminal.
- **HUD / Instrument** — Data overlays, status bars, reticles, diagnostic indicators, gauge-like displays. Flight instruments, vehicle dashboards, real-time monitoring tools.
- **Financial / Trading Terminal** — Extreme density, tabular data everywhere, semantic color (red/green), multi-pane windows. Bloomberg Terminal, TradingView, Interactive Brokers.
- **Scientific / Lab** — Measurement-forward, unit-labeled, precision type, SI-unit respect, diagrammatic composition. Lab instruments, scientific SaaS.

## Typefaces to Reach For

**Monospace (primary):** JetBrains Mono, IBM Plex Mono, Berkeley Mono, Fragment Mono, Fira Code, MonoLisa, Commit Mono, Söhne Mono.

**Technical sans:** Inter, Söhne, GT America, Aeonik, Neue Haas Grotesk — used in weights 400/500/600 only (weight hierarchy stays tight).

**Condensed sans for labels:** Söhne Schmal, GT America Condensed, Benton Sans Condensed — for short labels over data.

**Number-specific:** Any face with strong tabular figures. Most of the above offer `font-variant-numeric: tabular-nums`. Verify metrics.

## Palette Moves

- **Monochrome base** — a greyscale ramp from `#0F0F10` to `#F5F5F7` with 6–8 distinct steps for hierarchy without color.
- **Single signal color:** amber warning (`#FFB800`), diagnostic green (`#00E676`), warning red (`#FF3B30`), info blue (`#0A84FF`). One signal per screen usually.
- **HUD aesthetic:** Black base (`#000000`) with signal colors for status; white-on-black legibility.
- **Green-on-black terminal:** `#00FF41` or `#4ADE80` body on `#0A0A0A`.
- **Amber terminal:** `#FFB000` on `#0E0B07`.
- **Dashboard neutral:** Near-black (`#0A0B0D`) + light off-white card surfaces (`#F4F4F5`) + chart semantic colors (green positive, red negative, amber warning, blue info).
- **Dark mode is often the default** for this archetype — light mode takes more design effort to stay uncluttered.

Multiple subtle greys (6–8 distinct values) carry hierarchy where color would be noise. Tokens: `--grey-50` through `--grey-900`.

## Composition Moves

- **Dense data grids** with clear cell boundaries — `border: 1px solid var(--border-subtle)`. Sticky headers. Fixed-width columns with `table-layout: fixed`.
- **Sparklines, gauges, progress indicators** as first-class UI elements — not decoration, but primary data vehicles.
- **Visible 1 px divider rules** everywhere; tabular numerals in any number-containing column.
- **Status indicators** with precise positioning — LED-style dots, colored bars, semantic tags.
- **Readouts with labels + values + units** — `TEMP: 72.4°F`, `LATENCY: 243ms`, `THROUGHPUT: 1.2k req/s`. Units are always present.
- **Ruler-aligned marginalia** — tick marks, scale indicators, coordinate labels along axes.
- **Keyboard shortcuts visible** — `⌘K`, `⇧⌘P` shown in the UI as labeled mono badges.
- **Multi-pane layouts** that split the screen into functional regions (nav / main / detail / status bar at bottom).
- **Terminal prompts and command palettes** as interaction surfaces, even in non-CLI products.

## Motion Flavor

Instant or near-instant (0–150 ms). Utility over delight. Real-time data updates via subtle fade-in (100 ms) or number morph animation. Blinking cursor on active inputs (`animation: blink 1s steps(1) infinite`). Loading states are progress bars with precise percentages, not spinners. No decorative motion. Scroll is functional (no smooth-scroll hijack).

Exception: chart animations on initial data load can be 400–600 ms for readability — sparklines drawing in left-to-right communicates the data arrival.

## Depth & Texture

Flat almost everywhere. One elevation level for floating panels. Borders do the work that shadows would in other archetypes. Grain and texture largely absent — industrial is clean, precise, measured. Exception: HUD variant uses subtle scanlines, CRT tint, phosphor glow for atmosphere.

## Visual References

- **Digital now:** Linear (insights mode), Vercel dashboard, Datadog, Grafana, GitHub, Stripe dashboard, Warp terminal, Raycast, Superhuman, Retool, Arena (Are.na settings).
- **Financial:** Bloomberg Terminal (the gold standard of data density), TradingView, IBKR Workstation, Eikon.
- **Games:** Eve Online UI, Elite Dangerous, Kerbal Space Program, Returnal HUD, Death Stranding menus, Escape from Tarkov.
- **Hardware lineage:** Dieter Rams Braun instruments (T3, T1000), Teenage Engineering OP-1 + OP-Z, Nord synthesizers, Elektron drum machines, industrial control panels (lab, aerospace).
- **Designers:** Dieter Rams, Richard Sapper (Artemide/Tizio lamp, IBM ThinkPad), Teenage Engineering team, John Maeda (early computational design).
