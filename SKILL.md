---
name: frontend-design
description: Production-grade, bespoke frontend engineering with high design fidelity. Invoke for web components, pages, dashboards, applications, or any UI requiring polished visual execution. Outputs functional code with intentional aesthetic direction, accessibility, responsiveness, and performance-aware implementation.
---

# Frontend Design Skill

## Core Thesis

Great frontend design is disciplined translation: a clear, context-specific aesthetic intent (archetype + one differentiator) translated into a coherent system of typography, color tokens, layout, motion, and texture—implemented with accessibility, responsiveness, and performance as non-negotiables.

---

## 1. Operating Mode

Before writing code, complete this sequence:

1. **Context**: Identify purpose, users, domain, content density, and risk factors (accessibility/performance requirements). Output a clear problem statement.
2. **Aesthetic Direction**: Select one archetype from Section 2 and state it explicitly.
3. **Differentiator**: Define one memorable anchor—a signature interaction, typographic move, layout motif, texture, or material treatment.
4. **System**: Define tokens and rules: type scale, spacing rhythm, palette mapping, elevation levels.
5. **Implementation**: Outline structure and interaction model, then build.

**Directive:** Commit fully to the chosen direction. Do not average multiple styles into a bland middle. Hybridize only when you can articulate the governing rule for the hybrid.

---

## 2. Aesthetic Archetypes

Select one archetype as the foundation:

- **Editorial / Magazine**: Strong typographic hierarchy, generous whitespace, refined grid. Use pull quotes, drop caps, column layouts, and serif display type.
- **Swiss / International**: Geometric precision, sans-serif dominance, systematic spacing. Apply strict grids, Akzidenz/Helvetica lineage typefaces, and asymmetric balance.
- **Brutalist / Raw**: Exposed structure, high contrast, anti-decorative. Embrace monospace type, visible borders, system UI elements, and raw HTML aesthetic.
- **Minimalist / Refined**: Restraint, micro-contrast, meticulous spacing. Deploy limited palettes, ample whitespace, subtle shadows, and precise alignment.
- **Maximalist / Expressive**: Layered composition, bold color, dynamic motion, visual density. Use overlapping elements, animated gradients, and complex grid breaks.
- **Retro-Futuristic**: Nostalgic UI cues, neon accents, CRT aesthetics. Apply scanlines, glitch effects, terminal green, pixel fonts, and glow.
- **Organic / Natural**: Soft geometry, earthy palettes, tactile texture. Incorporate rounded shapes, grain overlays, hand-drawn elements, and warm tones.
- **Industrial / Utilitarian**: Functional aesthetic, monochrome, dense grids. Build data-heavy layouts with instrument-panel vibes and no ornamentation.
- **Art Deco / Geometric**: Symmetry, metallic accents, ornamental precision. Use fan shapes, gold/brass tones, decorative borders, and Gatsby-era typography.
- **Lo-Fi / Zine**: Rough textures, collage aesthetic, deliberate imperfection. Apply torn edges, mixed type, print artifacts, and halftone/duotone effects.

---

## 3. Technical Implementation

### 3.1 Typography

Choose context-appropriate typefaces that reinforce the archetype—avoid defaults like Arial, Inter, Roboto, and system stacks. Establish hierarchy through a distinct display/body pairing, using size, weight, case, and spacing to create 3–5 clear levels.

Use `clamp()` for fluid responsive scaling (e.g., `font-size: clamp(1rem, 2.5vw, 1.5rem)`). Tune `line-height` carefully: 1.4–1.6 for body text, 1.1–1.2 for display type. Adjust `letter-spacing` and `font-feature-settings` for refinement.

For loading, use `font-display: swap` and subset fonts to reduce payload.

### 3.2 Color System

Structure your palette with CSS custom properties: `--color-surface`, `--color-text`, `--color-muted`, `--color-primary`, `--color-accent`, `--color-border`. Add semantic tokens for feedback states: `--color-success`, `--color-warning`, `--color-error`.

Meet WCAG AA contrast minimums: 4.5:1 for normal text, 3:1 for large text and UI elements. Distribute color intentionally—dominant (60%) + supporting (30%) + accent (10%). Avoid timid, evenly-split palettes.

Implement theme support via `prefers-color-scheme` media query or explicit class toggle.

### 3.3 Motion & Interaction

Motion must communicate state, hierarchy, or affordance—never decoration alone. Use custom `cubic-bezier()` timing functions; avoid `linear` for UI transitions.

Orchestrate page-load sequences with staggered `animation-delay` offsets (50–100ms increments). For hardware acceleration, animate only `transform` and `opacity`—avoid animating `top`, `left`, `width`, or `height`.

Use `IntersectionObserver` for scroll-triggered animations; avoid scroll-jacking. Always honor `prefers-reduced-motion: reduce` with functional alternatives.

Prefer CSS for HTML/vanilla JS projects. Use Motion (Framer Motion) for React/Vue when available.

### 3.4 Spatial Composition

Use CSS Grid for 2D layouts and Flexbox for linear distribution. Define a consistent spacing scale with custom properties: `--space-xs`, `--space-sm`, `--space-md`, `--space-lg`, `--space-xl`.

Treat whitespace as a structural element, not leftover space. Create hierarchy through dramatic scale contrast (e.g., 4:1 heading-to-body ratio).

Break the grid intentionally—overlap elements with `position: absolute/relative` and `z-index` for purposeful disruption. Use asymmetric alignments to create visual tension; avoid defaulting to center alignment. Deploy full-bleed moments that break container boundaries for emphasis using viewport units.

### 3.5 Visual Depth & Texture

Build layered shadows with multiple `box-shadow` values using varying blur/spread for realistic depth. Define elevation levels: `--shadow-sm`, `--shadow-md`, `--shadow-lg`.

For glassmorphism, use `backdrop-filter: blur()` with semi-transparent backgrounds (check browser support). Add noise and grain via SVG `<feTurbulence>` filter or CSS `background-image` with texture overlay.

Create gradients with intention—mesh gradients, radial compositions, multi-stop configurations. Avoid generic purple→blue linear gradients.

Use `clip-path: polygon()` or `circle()` for non-rectangular shapes. Design borders and dividers with decorative intent, including custom `border-image` and creative separators that match the archetype.

Apply texture overlays appropriate to the style: halftone, duotone, or stipple for print aesthetics; scanlines for retro-futuristic.

---

## 4. Anti-Patterns

Explicitly avoid these markers of generic output:

**Typography**: Never use system font stacks, Inter/Roboto/Arial, or uniform sizing. Instead, choose distinctive, context-appropriate typefaces with clear hierarchy.

**Color**: Avoid purple-on-white gradients, evenly distributed palettes, and low contrast. Instead, commit to palettes with dominant/accent distribution and AA+ contrast.

**Layout**: Reject centered card grids and predictable hero→cards→testimonials→footer structures. Instead, use asymmetric compositions, unexpected grid breaks, and purposeful whitespace.

**Motion**: Eliminate gratuitous animations, linear easing, and motion without purpose. Instead, use purposeful transitions, custom easing, and orchestrated sequences.

**Details**: Remove stock illustrations, generic icons, and placeholder-style imagery. Instead, create bespoke graphics, custom iconography, and contextual imagery.

**Structure**: Never leave template scaffolding visible in final output. Deliver complete, polished implementations with no TODOs or placeholders.

---

## 5. Engineering Standards

### Accessibility (Non-negotiable)

Use semantic HTML elements appropriately: `<nav>`, `<main>`, `<article>`, `<section>`, `<button>`, `<form>`. Apply ARIA attributes only when native semantics are insufficient.

Ensure all interactive elements are reachable and operable via keyboard. Provide visible focus states that match the design system—never use `outline: none` without a replacement.

Write descriptive alt text for meaningful images; use empty alt for decorative images. Never convey information by color alone.

### Performance

Minimize render-blocking resources and inline critical CSS when appropriate. Subset fonts, use `font-display: swap`, and limit weights/variants.

Write efficient CSS selectors with maximum 3 levels of nesting. Keep animated surfaces small and minimize heavy blurs and large fixed layers.

Lazy-load off-screen images and heavy assets using appropriate image formats. Avoid unnecessary dependencies and tree-shake when using frameworks.

### Responsiveness

Build mobile-first CSS architecture. Use fluid units (`rem`, `em`, `vw`, `vh`, `%`, `clamp()`) over fixed pixels.

Set breakpoints based on content needs, not device categories. Ensure minimum 44x44px touch targets for interactive elements.

Include proper meta viewport tag and prevent horizontal scroll on mobile.

---

## 6. Output Contract

Every implementation must deliver:

- **Stated Direction**: Explicitly name the archetype and differentiator in 1–2 lines before code.
- **Working Code**: Complete, runnable snippet(s) appropriate to the chosen stack—no partial implementations.
- **Design Tokens**: CSS custom properties for colors, spacing, typography, and shadows.
- **Responsiveness**: Demonstrated via fluid layout, breakpoints, or container queries.
- **Accessibility**: Semantic structure, keyboard operability, and visible focus states.
- **Reduced Motion**: Explicit `prefers-reduced-motion` handling.

---

## 7. Finish Checklist

Before delivering, verify:

- **Archetype Fidelity**: Does every visual choice reinforce the stated archetype?
- **Differentiator**: Is the memorable anchor implemented, not just described?
- **Token Coherence**: Are typography, spacing, and color tokens consistent throughout?
- **Keyboard Access**: Can every interactive element be reached and used via keyboard?
- **Focus Visibility**: Are focus states visible and styled intentionally?
- **Responsive Behavior**: Does it remain intentional on mobile, tablet, and wide desktop?
- **Reduced Motion**: Is there a `prefers-reduced-motion` fallback?
- **Template Smell**: Is there any generic scaffolding remaining? Remove or transform it.
- **Placeholder Content**: Are there any TODOs, lorem ipsum, or placeholder comments? Remove them.
- **Contrast Compliance**: Do text and interactive elements meet WCAG AA contrast ratios?

---

Intention in every choice. Precision in every detail. Nothing left to default.
