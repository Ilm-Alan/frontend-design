# Frontend Design Skill for Claude Code, Codex, and Gemini CLI

An enhanced frontend design skill that produces production-grade UI code with high design fidelity. Works with [Claude Code](https://github.com/anthropics/claude-code) (Anthropic), [Codex](https://github.com/openai/codex) (OpenAI), and [Gemini CLI](https://github.com/google-gemini/gemini-cli) (Google). Replaces generic Bootstrap-looking output with intentional aesthetic direction, systematic design tokens, and polished visual execution.

## Features

- **10 aesthetic archetypes** — Editorial, Swiss, Brutalist, Minimalist, Maximalist, Retro-Futuristic, Organic, Industrial, Art Deco, Lo-Fi
- **Structured design process** — Context → Archetype → Differentiator → Token System → Implementation
- **Design token system** — CSS custom properties for colors, spacing, typography, shadows
- **Motion with purpose** — Custom easing, orchestrated sequences, scroll-triggered animations
- **Anti-pattern guidance** — Explicit list of generic markers to avoid
- **Quality checklist** — 5-point verification before delivery

## Installation

### Claude Code

```bash
mkdir -p ~/.claude/skills/frontend-design && curl -o ~/.claude/skills/frontend-design/SKILL.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/SKILL.md
```

### Codex

```bash
mkdir -p ~/.codex/skills/frontend-design && curl -o ~/.codex/skills/frontend-design/SKILL.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/SKILL.md
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
mkdir -p ~/.gemini/skills/frontend-design && curl -o ~/.gemini/skills/frontend-design/SKILL.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/SKILL.md
```

Run `/skills list` to verify the skill was loaded.

## Usage

Invoke the skill when requesting UI work:

```
/frontend-design Create a pricing page for a developer tools SaaS
```

Or reference it contextually:

```
Using the frontend design skill, build a dashboard for monitoring API usage
```

## Why Use This Instead of the Default Skill?

Anthropic ships a basic `frontend-design` skill with Claude Code. It encourages bold aesthetics but relies on inspiration over discipline:

> *"Pick an extreme: brutally minimal, maximalist chaos, retro-futuristic..."*

The problem: encouragement doesn't produce consistency. Without structure, outputs drift toward safe defaults—centered card grids, purple gradients, predictable layouts.

This skill provides the structure that makes creativity reliable.

| Aspect | Default Skill | This Skill |
|--------|---------------|------------|
| **Process** | "Commit to bold direction" | 5-step structured sequence |
| **Aesthetics** | "Pick an extreme" | 10 codified archetypes |
| **Design System** | "Use CSS variables" | Required token structure |
| **Anti-Patterns** | Brief warning | Explicit markers to avoid |
| **Verification** | None | 5-point checklist |

## The 10 Aesthetic Archetypes

| Archetype | Character |
|-----------|-----------|
| **Editorial / Magazine** | Strong typography, generous whitespace, refined grids, serif display type |
| **Swiss / International** | Geometric precision, systematic spacing, asymmetric balance, Helvetica lineage |
| **Brutalist / Raw** | Exposed structure, high contrast, monospace type, anti-decorative |
| **Minimalist / Refined** | Restraint, micro-contrast, meticulous spacing, limited palettes |
| **Maximalist / Expressive** | Layered composition, bold color, dynamic motion, visual density |
| **Retro-Futuristic** | CRT aesthetics, neon accents, scanlines, terminal green, pixel fonts |
| **Organic / Natural** | Soft geometry, earthy palettes, tactile texture, hand-drawn elements |
| **Industrial / Utilitarian** | Functional density, instrument-panel aesthetic, no ornamentation |
| **Art Deco / Geometric** | Symmetry, metallic accents, ornamental precision, Gatsby-era typography |
| **Lo-Fi / Zine** | Rough textures, collage aesthetic, deliberate imperfection, halftone effects |

## Output Contract

Every implementation delivers:

1. **Stated direction** — Named archetype + differentiator before code
2. **Working code** — Functional code that demonstrates the aesthetic direction
3. **Design tokens** — CSS custom properties for colors, spacing, typography, shadows
4. **Responsiveness** — Fluid layout with `clamp()`, breakpoints, or container queries

## Example

**Prompt:**
```
/frontend-design Build a command palette component for a code editor
```

**Output includes:**
```
Archetype: Brutalist / Raw
Differentiator: Phosphor-green monospace type with CRT text glow

[Functional implementation with tokens and responsive layout...]
```

## License

MIT. See [LICENSE.txt](LICENSE.txt).
