# frontend-design

Frontend design skill for Claude Code, Codex, and Gemini CLI. Eight anchors with binding CSS tokens — each engineered to escape the AI design default (cream paper, Fraunces serif, warm ink, one warm-red accent, paper grain).

## Install

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

## The problem this solves

Ask any AI coding assistant to "design a beautiful landing page" and it ships a five-token pattern: cream-paper surface + Fraunces or Garamond serif + warm near-black ink + one warm-red accent + 2–5% paper grain. Every ambiguous brief lands there. Different briefs, same production. Recognisable on sight as AI-slop.

The underlying issue: the default is baked into the statistical centre of "good design" in training data. Telling the model to be bold doesn't move it. Naming archetypes ("Swiss," "Brutalist") doesn't move it — the model adopts the label in the preamble and ships the default CSS anyway.

## How this skill works

The skill names the default explicitly, then offers eight anchors that escape it at the CSS token layer. Each anchor is a binding signature — specific palette, specific typefaces, specific texture. Picking an anchor commits to those tokens, not to a vibe.

Before writing code, the skill demands:

1. **Three candidate anchors**, with one sentence each on what each would do with the brief.
2. **A choice** — which anchor's grammar most directly serves the surface, and why.
3. **A differentiator** — one memorable move that's anchor-internal.
4. **Signature commitment** — the rendered CSS must match the anchor's binding tokens.

There is no Editorial anchor. If a brief genuinely needs magazine-register output, it is producible without invoking the skill. Omitting Editorial puts a tax on the default choice and clears the path for the alternatives.

## The eight anchors

| Anchor | Binding signature |
|---|---|
| **Swiss** | Pure white, Akzidenz/Helvetica/Söhne sans, Swiss Red or International Orange accent, visible grid |
| **Industrial** | Pitch black, IBM Plex Mono / JetBrains Mono throughout, one semantic signal color, flat |
| **Brutalist** | Pure primary colors, system fonts (Times, Helvetica, Courier), hard offset shadows `Xpx Xpx 0 #000`, native browser controls |
| **Aurora Maximalism** | Dark saturated gradient base, Inter/PP Neue Machina, mesh gradient surface, neon glow |
| **Chaotic Maximalism** | Clashing pastels + neons, mixed typefaces, patterns on every surface, oversized display |
| **Retro-Futuristic** | Pitch black + neon, period typefaces (VT323, Orbitron, Space Mono, Monoton), CRT scanlines or chromatic aberration |
| **Organic** | Earth tones (sage, clay, terracotta, ochre) — never cream, humanist serif or warm sans, rounded corners, subtle grain |
| **Lo-Fi** | Paper-yellow (not cream), mixed system fonts, rotated elements, halftone dots, Risograph misregistration |

Full binding signatures are in [`SKILL.md`](SKILL.md) §2.

## Repository structure

```
frontend-design/
├── SKILL.md
├── references/
│   ├── index.md      reading guide
│   ├── routing.md    domain-keyed candidate anchors
│   └── palettes.md   semantic-token palettes by domain and by mood
├── README.md
└── LICENSE.txt
```

## License

MIT.
