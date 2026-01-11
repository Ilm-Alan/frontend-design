# Frontend Design Skill

A structured skill for Claude Code and Codex that transforms the AI into a production-grade frontend engineer with high design fidelity. No more generic Bootstrap-looking output—this skill enforces intentional aesthetic direction, systematic design tokens, and polished visual execution.

## Why This Exists

Anthropic ships a basic `frontend-design` skill with Claude Code. It encourages bold aesthetics and warns against "AI slop," but relies on inspiration rather than discipline:

> *"Pick an extreme: brutally minimal, maximalist chaos, retro-futuristic..."*
> *"What makes this UNFORGETTABLE?"*
> *"Don't hold back, show what can truly be created"*

The problem: encouragement doesn't produce consistency. Without structure, outputs still drift toward safe defaults—centered card grids, purple gradients, predictable layouts. The basic skill tells Claude to be creative but doesn't tell it *how*.

This skill fixes that.

## What's Different

| Aspect | Basic Skill | This Skill |
|--------|-------------|------------|
| **Process** | "Understand context, commit to bold direction" | 5-step sequence: Context → Archetype → Differentiator → Token System → Implementation |
| **Aesthetic Direction** | Loose suggestions ("pick an extreme") | 10 codified archetypes with specific characteristics |
| **Design System** | "Use CSS variables for consistency" | Required token structure: `--color-surface`, `--space-md`, `--shadow-lg`, etc. |
| **Typography** | "Choose distinctive fonts" | Specific guidance: `clamp()` for fluid scaling, `line-height` ranges, `font-display: swap` |
| **Motion** | "Use animations for effects" | `cubic-bezier()` over `linear`, `IntersectionObserver` for scroll, `prefers-reduced-motion` handling |
| **Anti-Patterns** | Brief warning against generic aesthetics | Explicit list with alternatives for typography, color, layout, motion, and details |
| **Accessibility** | Not mentioned | Non-negotiable section: semantic HTML, ARIA, keyboard access, focus states, contrast ratios |
| **Performance** | Not mentioned | Dedicated section: critical CSS, font subsetting, selector efficiency, lazy loading |
| **Output** | Implicit expectations | 6-point contract: stated direction, working code, tokens, responsiveness, accessibility, reduced motion |
| **Verification** | None | 10-point finish checklist before delivery |

### The Core Improvement

The basic skill operates on **inspiration**: *"Be bold! Be creative! Don't hold back!"*

This skill operates on **discipline**: *"Complete this sequence. Define these tokens. Meet these standards. Verify against this checklist."*

Inspiration produces occasional brilliance and frequent mediocrity. Discipline produces consistent quality.

## Installation

### Claude Code

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git
mkdir -p ~/.claude/skills/frontend-design
cp frontend-design/skill.md ~/.claude/skills/frontend-design/
```

Or as a one-liner:

```bash
mkdir -p ~/.claude/skills/frontend-design && curl -o ~/.claude/skills/frontend-design/skill.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/skill.md
```

### Codex

```bash
git clone https://github.com/Ilm-Alan/frontend-design.git
mkdir -p ~/.codex/skills/frontend-design
cp frontend-design/skill.md ~/.codex/skills/frontend-design/
```

Or as a one-liner:

```bash
mkdir -p ~/.codex/skills/frontend-design && curl -o ~/.codex/skills/frontend-design/skill.md https://raw.githubusercontent.com/Ilm-Alan/frontend-design/main/skill.md
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

## The 10 Archetypes

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

1. **Stated direction**: Named archetype + differentiator in 1-2 lines before code
2. **Working code**: Complete, runnable—no partial implementations or TODOs
3. **Design tokens**: CSS custom properties for colors, spacing, typography, shadows
4. **Responsiveness**: Fluid layout with `clamp()`, breakpoints, or container queries
5. **Accessibility**: Semantic HTML, keyboard operability, visible focus states
6. **Reduced motion**: Explicit `prefers-reduced-motion` fallback

## Example

**Prompt:**
```
/frontend-design Build a command palette component for a code editor
```

**Output includes:**
```
Archetype: Brutalist / Raw
Differentiator: Phosphor-green monospace type with CRT text glow

[Complete implementation with tokens, accessibility, and reduced motion follows...]
```

## Philosophy

The basic skill's thesis: *"Claude is capable of extraordinary creative work. Don't hold back."*

This skill's thesis: *"Great frontend design is disciplined translation: a clear aesthetic intent translated into a coherent system of typography, color, layout, motion, and texture—implemented with accessibility, responsiveness, and performance as non-negotiables."*

Both are true. This skill provides the structure that makes the creativity reliable.

## License

MIT. See [LICENSE.txt](LICENSE.txt).
