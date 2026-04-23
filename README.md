# frontend-design

Frontend design skill for Claude Code, Codex, and Gemini CLI. Commits to one of ten aesthetic archetypes so the UI output looks chosen, not defaulted.

## Install

The skill is a folder (SKILL.md plus a references corpus), so install with `git clone`:

### Claude Code

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git ~/.claude/skills/frontend-design
```

### Codex

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git ~/.codex/skills/frontend-design
```

### Gemini CLI

Enable experimental skills in `~/.gemini/settings.json`:

```json
{ "experimental": { "skills": true } }
```

Then:

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git ~/.gemini/skills/frontend-design
```

Verify with `/skills list`.

## Use it

Invoke contextually in any UI prompt:

```
Using the frontend design skill, design a landing page for a Brooklyn punk record label
```

The skill names three candidate archetypes, picks one with stated reasoning, defines the type, palette, and texture system, and writes a single-file HTML+CSS document. The output begins with a short preamble naming every commitment.

## What it produces

For the punk-label prompt above, the preamble looks like:

```
Direction. Lo-Fi / Zine, Punk Flyer variant. The brief is a Brooklyn
hardcore label that refuses streaming and runs a basement venue; the
surface should look like it was photocopied at Kinko's in 1981 and
taped together on a kitchen table.

Values: anti-modernist. Coherence is the failure mode. Mixed faces
wielded as deliberate clash, halftone toner bleed, handwritten marker
on top of set type, stamps with uneven ink. Refinement would betray
the label.

Differentiator: a "NOT ON SPOTIFY" rubber stamp recurring nine times
across the page at inconsistent sizes and rotations.

Type: Times New Roman, Helvetica via Archivo Black, Courier, Georgia,
Impact. All system fonts wielded as style. Special Elite for the
typewritten manifesto, Permanent Marker for marginalia.

Palette: xeroxed-cream #EFE4C2, toner-black #0A0807, one shock-pink
Riso second pass #FF2E88. Three colors, no tuning.

Texture: SVG paper grain, halftone-dot record sleeves, rotated tape
strips, hard 6x6 ink-bleed shadows. Snap motion only.
```

Followed by a single-file HTML document implementing every choice.

## The ten archetypes

| Archetype | Values | Character |
|-----------|--------|-----------|
| Editorial / Magazine | Modernist | Strong typography, refined grid, generous whitespace |
| Swiss / International | Modernist | Geometric precision, sans-serif, systematic spacing |
| Minimalist / Refined | Modernist | Restraint, micro-contrast, meticulous spacing |
| Industrial / Utilitarian | Modernist | Functional density, instrument-panel, monochrome with signal color |
| Art Deco / Geometric | Modernist (ornamental) | Symmetry, metallic accents, ornamental precision |
| Maximalist / Expressive | Modernist (Aurora) or anti-modernist (Memphis) | Layered composition, saturated color, dynamic motion |
| Retro-Futuristic | Hybrid: nostalgic precision | CRT, neon, scanlines, synthwave and cyberpunk |
| Organic / Natural | Hybrid: warmth-as-discipline | Soft geometry, earthy palettes, hand-drawn marks |
| Brutalist / Raw | Anti-modernist | System fonts as style, exposed structure, anti-decoration |
| Lo-Fi / Zine | Anti-modernist | Rough texture, deliberate clash, photocopier artifacts |

## Why this and not the default skill

Anthropic ships a `frontend-design` skill with Claude Code that encourages bold direction. In practice it funnels to polished Editorial when the brief is ambiguous, because its evaluation criteria (coherence, refinement, intention) are themselves modernist values. Archetypes that reject those values, like Brutalist and Lo-Fi, fail the skill's own checks even when they fit the brief better. The result is a skill that lists ten archetypes but tends to produce variations of one.

This skill names that bias and rebuilds around it:

- The model picks an archetype after considering three candidates against the brief, using a domain-keyed reference (`references/routing.md`).
- Each archetype is tagged as modernist, anti-modernist, or hybrid, and the model names the stance in the output preamble.
- The procedure splits at the system step. Modernist archetypes commit to refined craft (specific typefaces, cited palettes, smooth motion). Anti-modernist archetypes commit to anti-craft (system fonts wielded as style, deliberate clash, snap motion). Per-archetype values commitments live in `references/values.md`.
- The references folder is four files: `routing.md`, `values.md`, `palettes.md`, and `index.md` (reading guide). Each is consulted at a specific decision point in the operating mode.

In practice you get a Brutalist record-label page that ships Times New Roman with `box-shadow: 6px 6px 0 #000`, not Editorial dressed up with a punk theme. You get an Industrial dashboard in IBM Plex Mono with no grain overlay, not an editorial broadsheet pretending to be data. Different artifacts across archetypes, not the same one in different costumes.

## Repository structure

```
frontend-design/
├── SKILL.md
├── references/
│   ├── index.md      reading guide for the model
│   ├── routing.md    domain-keyed candidate archetypes for the deliberation step
│   ├── values.md     per-archetype values commitments; supersedes §3 for anti-modernist
│   └── palettes.md   semantic-token palettes by product domain and by mood
├── README.md
└── LICENSE.txt
```

## License

MIT. See [LICENSE.txt](LICENSE.txt).
