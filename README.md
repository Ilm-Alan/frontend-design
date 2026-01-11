# Frontend Design Skill for Claude Code and Codex

An enhanced frontend design skill that produces production-grade UI code with high design fidelity. Works with both [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (Anthropic) and [Codex](https://github.com/openai/codex) (OpenAI). Replaces generic Bootstrap-looking output with intentional aesthetic direction, systematic design tokens, and polished visual execution.

## Features

- **10 aesthetic archetypes** — Editorial, Swiss, Brutalist, Minimalist, Maximalist, Retro-Futuristic, Organic, Industrial, Art Deco, Lo-Fi
- **Structured design process** — Context → Archetype → Differentiator → Token System → Implementation
- **Design token system** — CSS custom properties for colors, spacing, typography, shadows
- **Accessibility built-in** — Semantic HTML, ARIA, keyboard navigation, focus states, WCAG contrast
- **Performance standards** — Critical CSS, font optimization, efficient selectors, lazy loading
- **Motion with purpose** — Custom easing, orchestrated sequences, `prefers-reduced-motion` support
- **Quality checklist** — 10-point verification before delivery

## Installation

### Claude Code

```bash
mkdir -p ~/.claude/skills/frontend-design && curl -o ~/.claude/skills/frontend-design/SKILL.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/SKILL.md
```

### Codex

```bash
mkdir -p ~/.codex/skills/frontend-design && curl -o ~/.codex/skills/frontend-design/SKILL.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/SKILL.md
```

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
| **Accessibility** | Not mentioned | Non-negotiable standards |
| **Performance** | Not mentioned | Dedicated requirements |
| **Verification** | None | 10-point checklist |

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
2. **Working code** — Complete, runnable, no TODOs or placeholders
3. **Design tokens** — CSS custom properties for colors, spacing, typography, shadows
4. **Responsiveness** — Fluid layout with `clamp()`, breakpoints, or container queries
5. **Accessibility** — Semantic HTML, keyboard operability, visible focus states
6. **Reduced motion** — Explicit `prefers-reduced-motion` fallback

## Example

**Prompt:**
```
/frontend-design Build a command palette component for a code editor
```

**Output includes:**
```
Archetype: Brutalist / Raw
Differentiator: Phosphor-green monospace type with CRT text glow

[Complete implementation with tokens, accessibility, and reduced motion...]
```

## License

MIT. See [LICENSE.txt](LICENSE.txt).
