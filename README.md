# frontend-design

Frontend design skill for Claude Code, Codex, and Gemini CLI. Eight aesthetic anchors, each locking palette, typography, and texture to specific CSS tokens. Pick one per brief.

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

## How it works

Each anchor locks specific palette, typefaces, and texture tokens. Picking an anchor commits to those tokens, not to a vibe. Before any code, the skill asks for:

1. Three candidate anchors considered against the brief.
2. A choice, with reasoning in one line.
3. A memorable anchor-internal move.
4. CSS that matches the chosen anchor's tokens.

If the rendered tokens drift outside the anchor's range, the anchor didn't hold.

## The eight anchors

| Anchor | Tokens |
|---|---|
| **Swiss** | Pure white, Akzidenz/Helvetica/Söhne sans, Swiss Red or International Orange accent, visible grid |
| **Industrial** | Pitch black, IBM Plex Mono / JetBrains Mono throughout, one semantic signal color, flat |
| **Brutalist** | Pure primary colors, system fonts (Times, Helvetica, Courier), hard offset shadows `Xpx Xpx 0 #000`, native browser controls |
| **Aurora Maximalism** | Dark saturated gradient base, Inter/PP Neue Machina, mesh gradient surface, neon glow |
| **Chaotic Maximalism** | Clashing pastels + neons, mixed typefaces, patterns on every surface, oversized display |
| **Retro-Futuristic** | Pitch black + neon, period typefaces (VT323, Orbitron, Space Mono, Monoton), CRT scanlines or chromatic aberration |
| **Organic** | Earth tones (sage, clay, terracotta, ochre) — never cream, humanist serif or warm sans, rounded corners, subtle grain |
| **Lo-Fi** | Paper-yellow (not cream), mixed system fonts, rotated elements, halftone dots, Risograph misregistration |

Full token specs are in [`SKILL.md`](SKILL.md).

## Repository structure

```
frontend-design/
├── SKILL.md
├── README.md
└── LICENSE.txt
```

## License

MIT.
