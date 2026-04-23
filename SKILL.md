---
name: frontend-design
description: Bespoke frontend engineering focused purely on aesthetic excellence — modernist or anti-modernist, whichever the chosen archetype demands. Invoke for web components, pages, dashboards, applications, or any UI requiring distinctive visual execution. Outputs functional code with full commitment to the archetype's values, refining or refusing refinement as the direction calls for.
---

# Frontend Design Skill

## Core Thesis

Great frontend design is a committed answer to *what this surface wants to be*. The answer might be discipline (refined typography, coherent system, intention in every detail). It might be chaos (deliberate clash, productive contradiction, system fonts wielded as style). It might be friction (visible structure, snap motion, anti-decoration). It might be ornament, nostalgia, deliberate imperfection — depending on the archetype the brief calls for.

**Each archetype carries its own values.** Modernist archetypes — Editorial, Swiss, Minimalist, Industrial, Art Deco — reward refinement, coherence, and intention. Anti-modernist archetypes — Brutalist, Lo-Fi, chaotic Maximalism — reward roughness, contradiction, and deliberate mess. Hybrid archetypes — Retro-Futuristic, Organic, modernist Maximalism — operate by their own value systems (nostalgic precision, warmth-as-discipline, ambitious-but-coherent layering).

Commit to the archetype's *values* as fully as you commit to its visual moves. The failure modes are symmetric: producing anti-modernist work modernistically (a sanitised Brutalism, a polished Lo-Fi, a coherent Memphis-Maximalism) and producing modernist work without commitment (a watered-down Editorial). Both are betrayals of the chosen direction.

Reference material lives in `references/`. Four files: `routing.md` (domain-keyed archetype routing), `values.md` (per-archetype values commitments), `palettes.md` (semantic-token palettes by domain and by mood), `index.md` (reading guide). The SKILL.md carries the decision procedure; references supplement it at specific decision points named in §1.

---

## 1. Operating Mode

Before writing code, complete this sequence:

1. **Context** — Identify purpose, audience, domain, and content density. State the problem in one sentence.
2. **Aesthetic Direction** — Before committing, name three candidate archetypes that could fit this brief and one sentence on what each would do with it. Consult `references/routing.md` to ground candidates in the surface's grammar. Pick the candidate whose grammar most directly serves the brief's content and purpose. State the chosen archetype, **its values stance** (modernist / anti-modernist / hybrid), and the reason in one line.
3. **Differentiator** — Define one memorable anchor: a signature interaction, typographic move, layout motif, texture, or material treatment. Pick something the archetype rewards and the brief specifically earns; the differentiator should be describable in one sentence and visible in the rendered output.
4. **System** — Translate the chosen direction into specific commitments. The interpretation depends on the archetype's values (see `references/values.md` for the per-archetype specifics):
   - **For modernist archetypes** (Editorial, Swiss, Minimalist, Industrial, Art Deco, modernist Maximalism): pick a specific display/body pairing by face name. Derive a palette from `references/palettes.md` (by-domain or by-mood section) with any tuning named. Texture stays flat unless `values.md` names a texture move for the archetype. Spacing, elevation, and motion follow the §3 modernist craft rules below.
   - **For anti-modernist archetypes** (Brutalist, Lo-Fi, chaotic Maximalism): commit to the archetype's *anti-craft*. System fonts wielded with conviction (Brutalist), mixed faces selected for collision (Lo-Fi), oversized expressive display in productive clash (chaotic Maximalism). **`values.md` supersedes the §3 modernist defaults below for these archetypes — work from it directly.**
   - **For hybrid archetypes** (Retro-Futuristic, Organic): `values.md` names the specific value system; follow it.
5. **Implementation** — Outline structure and interaction model, then build.

Commit fully to the chosen direction *and its values*. Hybridize only when you can articulate the governing rule for the hybrid.

---

## 2. Aesthetic Archetypes

Each archetype belongs to a kind of surface — its grammar fits some briefs and pulls against others. Match the archetype to the brief's content and purpose:

- **Text-led** (publications, long-form, brand storytelling, considered reading) → Editorial, Lo-Fi
- **Clarity-led** (documentation, brand systems, modern tech) → Swiss, Minimalist
- **Data-led** (dashboards, observability, analytics, financial terminals) → Industrial, Swiss
- **Warmth-led** (wellness, food, craft, lifestyle) → Organic, Minimalist
- **Spectacle-led** (creative agencies, gaming, music, brand experiences, hero campaigns) → Maximalist, Retro-Futuristic
- **Restraint-led** (luxury, premium consumer, considered tech) → Minimalist, Editorial
- **Edge-led** (indie tools, anti-design, intentional friction, punk-adjacent) → Brutalist, Lo-Fi
- **Nostalgia-led** (gaming, music, period-evocative) → Retro-Futuristic, Art Deco
- **Opulence-led** (hospitality, fashion, fragrance, period-appropriate) → Art Deco, Editorial

The list below is alphabetical with each archetype tagged by its values stance. For domain-keyed archetype guidance, read `references/routing.md`. For per-archetype values commitments and the modernist-defaults override (Brutalist, Lo-Fi, chaotic Maximalism), read `references/values.md`.

- **Art Deco / Geometric** [modernist with ornament] — Symmetry, metallic accents, ornamental precision.
- **Brutalist / Raw** [anti-modernist] — Exposed structure, system defaults wielded as style, anti-decoration.
- **Editorial / Magazine** [modernist] — Strong typographic hierarchy, refined grid, generous whitespace.
- **Industrial / Utilitarian** [modernist] — Functional aesthetic, monochrome, dense data grids, instrument-panel energy.
- **Lo-Fi / Zine** [anti-modernist] — Rough texture, deliberate clash, photocopier artifacts, productive imperfection.
- **Maximalist / Expressive** [modernist (Aurora, Liquid Glass) OR anti-modernist (Memphis, Vibrant Block)] — Layered composition, saturated color, dynamic motion, visual density. Pick the sub-mode in §1.2 — they have opposite values.
- **Minimalist / Refined** [modernist] — Restraint, micro-contrast, meticulous spacing, precise alignment.
- **Organic / Natural** [hybrid: warmth-as-discipline] — Soft geometry, earthy palette, tactile texture, hand-drawn marks.
- **Retro-Futuristic** [hybrid: nostalgic precision] — Nostalgic UI cues, neon accents, CRT texture, synthwave/cyberpunk lineage.
- **Swiss / International** [modernist] — Geometric precision, sans-serif dominance, systematic spacing, numerical composition.

---

## 3. The Modernist Aesthetic System

The principles below describe **modernist craft** — refinement, coherence, intention. They apply to Editorial, Swiss, Minimalist, Industrial, Art Deco, and modernist Maximalism (Aurora, Liquid Glass, 3D / Hyperrealism).

For **anti-modernist archetypes** (Brutalist, Lo-Fi, chaotic Maximalism), `references/values.md` supersedes the principles below. Skip §3 and work from `values.md` directly.

For **hybrid archetypes** (Retro-Futuristic, Organic), apply §3 as far as the archetype's value system supports. `values.md` names where it diverges.

### 3.1 Typography

Choose typefaces that carry the archetype. Pair a distinctive display face with a body face — scale, weight, case, and tracking build 3–5 clear hierarchy levels. Let body fall back to a system stack only where the display face already carries the identity alone.

Set type fluidly across viewport sizes. Tune line-height to 1.45–1.65 for body and 1.05–1.2 for display. Use tabular figures for aligned numerics. Tighten tracking at display sizes; let body breathe at default tracking or slightly open.

Create dramatic scale contrast between display and body — aim for ~4:1 or higher. Let hierarchy emerge from weight, case, tracking, and scale working together.


### 3.2 Typographic Craft

Align type optically rather than geometrically. The period after a digit sits a hair higher than a comma; capital letters need their own optical baseline against lowercase; hanging punctuation pulls quote marks outside the column edge so body text aligns true.

Use italic as counterpoint, rather than only as emphasis — a different voice for asides, captions, attribution, and quotation. Reach for small caps and old-style figures where the typeface offers them. Activate the ligatures the face supports.

Open up tracking on display caps (`+0.05em` to `+0.2em` for editorial, wider for Art Deco letter-spaced caps). Tighten it at hero display sizes (`-0.02em` to `-0.04em`). Let body tracking stay native to the typeface.

### 3.3 Color

Distribute color with 60/30/10 dominance — one lead surface, one supporting field, one accent that earns attention. Derive the palette from the product domain and emotional register: trust-blue for SaaS, deep ink with gold for luxury, saturated primaries for playful B2C, desaturated neutrals with one ink accent for editorial.

The palette has roles — surface, foreground, primary, accent, muted, border, plus the semantic states — and every component draws from those roles consistently rather than reinventing the palette per surface.

Design light and dark variants as a pair, tuned per archetype. Dark mode shifts tonally with desaturated surfaces and temperature-calibrated darks — a treatment to compose, rather than an inversion of light mode.

For specific palettes with hex values, consult `references/palettes.md` — domain-keyed in the first half, mood-keyed in the second.

### 3.4 Color Theory

Color thinking happens on three axes: **value** (light to dark), **chroma** (saturated to neutral), and **temperature** (warm to cool). A coherent palette varies one or two of these axes while holding the third — vary value across a near-monochrome scheme, vary chroma against held value for emotional register, vary temperature for warmth or coolness.

Harmonic structures set the tension level: **analogous** (calm), **complementary** (high tension), **triadic** (balanced energy), **split-complementary** (energetic without aggression), **monochromatic** (meditative). Match the harmonic to the archetype's emotional register.

Account for **simultaneous contrast** — a color reads differently against different surrounds. Test colors in their intended context. Account for **value over hue** — a composition that holds together in greyscale will hold together in color.

### 3.5 Composition

Treat whitespace as a structural element, rather than leftover space. The page reads as a *figure-ground* composition — what is figure and what is ground is decided.

Compose for visual rhythm: regular spacing intervals create calm; irregular intervals with intent create emphasis. Build tension through scale contrast, density contrast, alignment shifts. Release that tension before the next composition demands attention — every section earning emphasis dilutes the emphasis.

Use asymmetric alignment by default. Commit to overlapping motifs across the whole composition. Deploy full-bleed sections to mark transitions and emphasize scale shifts. Spacing rhythm flows from a shared scale (4 pt or 8 pt base); depth flows from a shared elevation order.

### 3.6 Motion

Motion expresses state, hierarchy, or causality. Choose easing that matches the archetype — custom curves for refined UI, spring physics where the archetype calls for material weight.

Timing as craft: 150–250 ms for micro-interactions, 200–400 ms for component transitions, ~500 ms for orchestrated reveals. Exits run shorter than enters. Stagger list and grid entrance by 30–50 ms per item.

Smooth motion comes from animating compositor properties — transform and opacity carry weight without forcing the page to redraw. Orchestrate page entrance with staggered timings. Reveal scroll content as it enters the viewport. Carry continuity between scenes with shared-element transitions where the metaphor calls for it.

Motion flavor is archetype-specific — quiet crossfades for editorial, spring physics for maximalist, snap for brutalist (see `values.md` for the anti-modernist motion stances).

### 3.7 Depth & Texture

Depth implies light. A consistent light source casts consistent shadows. Build layered shadows with varied blur and spread for real dimension. Decide elevation order once and apply it everywhere — cards, sheets, and modals share the same vocabulary of altitude.

Glass surfaces blur the field beneath, suggesting layers of material. Grain warms surfaces with tactile noise. Non-rectangular silhouettes through clipping or custom borders break the rectangle and mark identity. Mesh or radial gradients carry mood through atmospheric field, rather than as ornament added on top.

Texture is archetype-specific. Surfaces stay flat by default. Apply grain, scanlines, glass blur, halftone, duotone, exposed seams, or iridescence only when the archetype calls for it: halftone or duotone for print-inflected styles, scanlines for retro-futuristic, film grain for organic, exposed seams for brutalist, iridescence for maximalist. Industrial and Swiss treat flatness as identity.

---

## 4. Output Contract

Every implementation delivers:

- **Stated direction** — A short preamble *in a designer's prose* before the code, naming the choices with conviction. Name the archetype, its **values stance**, and why; name the differentiator and what it does; name the type pairing (display + body, by face name, OR system fonts wielded as style for anti-modernist work); name the palette source and any tuning (or the deliberate clash for anti-modernist work); state the texture stance. Read it back: would a designer recognise their voice in it, or does it read as a checklist?

  *Voice for modernist work:*
  > **Direction.** Industrial / Observability — the brief's verb is *measure*, and the surface is an instrument face, not a story. **Values:** modernist — refinement, coherence, intention. **Differentiator:** a calibrated tick-rule running across the masthead and threading every card edge — the dashboard reads as one continuous instrument. **Type:** IBM Plex Mono throughout for numerals and labels; Inter only for the one prose paragraph. **Palette:** derived from the Financial Dashboard entry — warm-black `#0B0C0A`, bone foreground, acid-lime signal `#C6FF4A` for the live series, amber `#F5B338` for drift. **Texture:** flat. Industrial holds flatness as identity.

  *Voice for anti-modernist work:*
  > **Direction.** Brutalist / Raw — the brief is a punk record label, and the surface should refuse polish. **Values:** anti-modernist — anti-decoration, exposed structure, system defaults as deliberate style. **Differentiator:** every interactive element is a default browser button (no custom styles) on a `#FFFF00` field, and underlined links stay web-default-blue. **Type:** Times New Roman for body, Helvetica Black at 200pt for display — both shipping system fonts, both wielded with conviction. **Palette:** pure `#000000`, pure `#FFFFFF`, pure `#FF0000`. No tuning. **Texture:** none — the page refuses finish. Hard drop-shadows (`box-shadow: 8px 8px 0 #000`) are the only depth, and they announce themselves as graphic.

- **Visible commitment** — Every choice in the rendered output traceable to the archetype and its values. The aesthetic shows, rather than only being stated.
- **Coherent commitment** — Modernist archetypes show coherence as token consistency (palette, type rhythm, spacing, elevation, motion expressed as shared rules). Anti-modernist archetypes show coherence as **consistent commitment to the archetype's anti-craft** — every visible element refusing the same things in the same way.

---

## 5. Intention Check

Before delivering:

- **Archetype deliberation** — Did I name three candidates and reason about fit before committing, rather than reaching for the first that came to mind?
- **Values commitment** — Did I commit to the archetype's *actual* values? Modernist archetypes demand refinement and coherence; anti-modernist archetypes demand roughness and productive contradiction. Compromising either way is the failure mode.
- **Archetype fidelity** — Can I name the archetype behind each visible choice? For anti-modernist work, can I also name what each choice is *refusing*?
- **Differentiator** — Is the memorable anchor actually implemented in the rendered output, rather than only described?
- **Specificity** — Are choices deliberate? Modernist deliberation = named typefaces from the catalog, cited palette entries, tuned hex values. Anti-modernist deliberation = system defaults wielded with conviction, deliberate mismatch, unapologetic primaries. Both are specificity.
- **Voice** — Does the preamble read as a designer naming their choices, with conviction, rather than as a checklist?
- **Template resistance** — Does any visible choice read as scaffolding rather than expression? Transform it until it carries the archetype.

Intention in every choice. Precision in every detail — including the precision of deliberate imperfection. The archetype carries identity; *its values* shape what counts as success.
