# Frontend Design Skill for Claude Code, Codex, and Gemini CLI

A frontend design skill that produces aesthetically committed UI code across the full archetype range — from refined modernist work (Editorial, Swiss, Industrial) to genuinely anti-modernist commitment (Brutalist, Lo-Fi, chaotic Maximalist). Works with [Claude Code](https://github.com/anthropics/claude-code) (Anthropic), [Codex](https://github.com/openai/codex) (OpenAI), and [Gemini CLI](https://github.com/google-gemini/gemini-cli) (Google).

The previous version produced Editorial-flavoured outputs across most briefs because its evaluation criteria — coherence, refinement, intention — were themselves modernist values that filtered out anti-modernist archetypes. The skill claimed 10 archetypes but could only execute 5. This release names that bias and rebuilds around values pluralism: each archetype carries its own values, and the skill commits to those values as fully as it commits to visual moves.

## What changed

- **Values-pluralist core thesis** — discipline, chaos, friction, ornament, deliberate imperfection are all valid commitments depending on the archetype the brief calls for
- **Values stance per archetype** — modernist (Editorial, Swiss, Minimalist, Industrial, Art Deco), anti-modernist (Brutalist, Lo-Fi, chaotic Maximalist), hybrid (Retro-Futuristic, Organic)
- **Bifurcated procedure** — modernist archetypes follow refined craft (named typefaces, cited palettes, smooth motion); anti-modernist archetypes commit to *anti-craft* (system fonts wielded as style, deliberate clash, snap motion)
- **Three-candidate deliberation** — the skill names 3 candidate archetypes and reasons about fit before committing, defusing the default-attractor bias
- **Rich on-demand reference corpus** — 10 archetype reference files, 25+ product-domain palettes, 15 mood-keyed palettes, 32 display/body type pairings, 50+ signature differentiators across 7 categories, domain-keyed archetype routing
- **Designer's prose preamble** — every output names archetype, values stance, differentiator, type pairing, palette source, and texture stance in conviction-prose, not as a checklist
- **Charter purity** — purely aesthetic excellence; accessibility, platform-correctness, and state-coverage belong to separate skills

## Installation

The skill now ships as a multi-file bundle (SKILL.md + references/), so the single-file `curl` install no longer works. Use git clone:

### Claude Code

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git ~/.claude/skills/frontend-design
```

### Codex

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git ~/.codex/skills/frontend-design
```

### Gemini CLI

First, enable the experimental skills feature in `~/.gemini/settings.json`:

```json
{
  "experimental": {
    "skills": true
  }
}
```

Then install the skill:

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git ~/.gemini/skills/frontend-design
```

Run `/skills list` to verify the skill was loaded.

## Usage

Invoke the skill when requesting UI work:

```
/frontend-design Design a landing page for a punk record label
```

Or reference it contextually:

```
Using the frontend design skill, build a dashboard for an institutional trading platform
```

The skill names three candidate archetypes, picks one with stated reasoning (committing to its values stance), defines the type/palette/texture system from the reference catalog, and produces a single-file HTML+CSS document with a designer's-prose preamble.

## Why use this instead of the default skill?

Anthropic ships a basic `frontend-design` skill with Claude Code. It encourages bold aesthetics but treats archetype as a label, not a values commitment. The result is convergence on a Western-modernist canon regardless of brief, because the evaluation criteria are themselves modernist. This skill names the bias and rebuilds the procedure to support both modernist and anti-modernist work.

| Aspect | Default skill | This skill |
|--------|---------------|------------|
| **Process** | "Commit to bold direction" | 5-step structured sequence with explicit deliberation |
| **Aesthetics** | "Pick an extreme" | 10 codified archetypes with values-stance tagging |
| **Selection bias** | Defaults to "design beautifully" | 3-candidate deliberation grounded in domain reference |
| **Reference depth** | None | ~1,900 lines of style/palette/typography/differentiator references |
| **Anti-modernist reach** | Rare; outputs converge on modernist | First-class — Brutalist and Lo-Fi outputs that refuse polish |
| **Output preamble** | None required | Designer's prose naming every system commitment |

## The 10 Aesthetic Archetypes

| Archetype | Values stance | Character |
|-----------|---------------|-----------|
| **Editorial / Magazine** | Modernist | Strong typography, refined grid, generous whitespace, print sensibility |
| **Swiss / International** | Modernist | Geometric precision, sans-serif dominance, systematic spacing |
| **Minimalist / Refined** | Modernist | Restraint, micro-contrast, meticulous spacing, precise alignment |
| **Industrial / Utilitarian** | Modernist | Functional density, instrument-panel energy, monochrome with signal color |
| **Art Deco / Geometric** | Modernist (ornamental) | Symmetry, metallic accents, ornamental precision |
| **Maximalist / Expressive** | Modernist (Aurora) OR anti-modernist (Memphis) | Layered composition, saturated color, dynamic motion |
| **Retro-Futuristic** | Hybrid: nostalgic precision | CRT aesthetics, neon accents, scanlines, synthwave/cyberpunk |
| **Organic / Natural** | Hybrid: warmth-as-discipline | Soft geometry, earthy palettes, tactile texture, hand-drawn marks |
| **Brutalist / Raw** | Anti-modernist | System defaults wielded as style, exposed structure, anti-decoration |
| **Lo-Fi / Zine** | Anti-modernist | Rough texture, deliberate clash, photocopier artifacts, productive imperfection |

## What "anti-modernist" actually means

Three archetypes (Brutalist, Lo-Fi, chaotic Maximalism) reject the premises modernist craft is built on:

- System fonts (Times, Helvetica, Courier, Marker Felt) wielded *as deliberate style*, not as fallback
- Deliberate clash and unapologetic primaries rather than coherent 60/30/10 palettes
- Snap motion (`steps(1)`, 0 ms transitions) rather than smooth compositor easing
- Hard offset shadows that announce themselves as graphic, not material light
- Off-grid placement, rotated elements, photocopier artifacts as the aesthetic

In the previous version, these were catalogued but unreachable — a "Brutalist" output came out as a polished Editorial site with a punk theme, because the skill's evaluation criteria rejected anti-craft as failure. This version's bifurcated procedure lets the skill commit to anti-modernist work without failing its own checks. A Brutalist landing page now reads like Are.na or pre-redesign Gumroad, not like a sanitised approximation.

## Repository structure

```
frontend-design/
├── SKILL.md                          The skill prompt (~170 lines)
├── references/
│   ├── styles/
│   │   ├── editorial.md, swiss.md, brutalist.md, minimalist.md,
│   │   ├── maximalist.md, retro-futuristic.md, organic.md,
│   │   └── industrial.md, art-deco.md, lo-fi.md
│   ├── palettes/
│   │   ├── by-domain.md              25+ product-type palettes with semantic tokens
│   │   └── by-mood.md                15 mood-keyed palettes
│   ├── typography/
│   │   └── pairings.md               32 display/body type pairings
│   ├── differentiators.md            50+ signature anchor moves
│   └── archetype-by-domain.md        Domain-keyed archetype routing
├── README.md
└── LICENSE.txt
```

## Output Contract

Every implementation delivers:

1. **Stated direction** — A short preamble in designer's prose naming the archetype, its values stance, the differentiator, the type pairing, the palette source, and the texture stance — written with conviction, not as a checklist
2. **Visible commitment** — Every choice in the rendered output traceable to the archetype and its values
3. **Coherent commitment** — Modernist archetypes show coherence as token consistency (palette, type rhythm, spacing, elevation, motion); anti-modernist archetypes show coherence as consistent commitment to the archetype's anti-craft

## Example

**Prompt:**
```
/frontend-design Design a landing page for a Brooklyn-based punk and hardcore record label
```

**Stated direction:**
```
Direction. Lo-Fi / Zine — Punk Flyer variant — because the brief is the
aesthetic: hardcore, vinyl-only, basement venue, refusal as a posture.

Values: anti-modernist — deliberate clash, photocopier roughness,
anti-decoration, every move refusing something the streaming-era web
takes for granted.

Differentiator: a "NOT ON SPOTIFY" rubber stamp that recurs nine times
across the page at deliberately inconsistent sizes and rotations.

Type: Times New Roman, Impact, Helvetica Black slammed against Courier,
Marker Felt for handwriting overlays — all shipping system fonts wielded
as style, none commissioned, none web-loaded. The clash is the move.

Palette: xeroxed-cream paper #EFE4C2, toner-black #0A0807, one shock-pink
Riso second pass #FF2E88. No tuning beyond ink-bleed.

Texture: heavy SVG paper grain, halftone-dot record sleeves, rotated tape
strips, hard 6px 6px 0 #000 ink-bleeds, every block 1–6° off-grid.
Snap motion only — no easing curves anywhere. The page refuses finish.
```

(Followed by a single-file HTML document implementing every commitment named.)

## License

MIT. See [LICENSE.txt](LICENSE.txt).
