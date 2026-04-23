# Differentiators — A Catalog of Memorable Anchors

The differentiator is the one move you can describe in a sentence that someone would remember after closing the tab. Not the whole design — the *anchor*. Pick one per project; commit to it across every screen where it applies.

This catalog organizes signature moves by category. Each is a starting point — adapt to the archetype, not the other way around.

---

## Signature Interactions

**Magnetic cursor / button pull** — Buttons subtly attract the cursor when it nears, with spring physics. Implement via mouse position + transform translate, dampened. Strong fit: Maximalist, Tech Minimalist (Linear, Arc).

**Cursor-following gradient** — A soft radial gradient follows the mouse, lighting the surface beneath. Use `radial-gradient` positioned via CSS variables updated on `mousemove`. Strong fit: Maximalist, Premium Tech.

**Custom cursor** — Replace the default cursor with a circle, dot, plus-sign, or context-shifting shape. The cursor itself becomes brand. Strong fit: Maximalist, Editorial-Modern (Bibliothèque-style).

**Cursor trails** — Particle or color trails follow cursor movement. Subtle is critical — over-implemented becomes nauseating. Strong fit: Maximalist, Retro-Futurist.

**Scroll-linked color shift** — Page background animates from one palette to another as the user scrolls. Use `IntersectionObserver` or CSS scroll-driven animations. Strong fit: Editorial, Maximalist, Brand storytelling.

**Scroll-progress reveal** — Long-form content where each section reveals an element synchronized with scroll position (parallax, image stacking, type morph). Strong fit: Editorial, Maximalist, Marketing storytelling.

**Hover sound** — Subtle audio feedback on key interactions. Used carefully (default-muted; obvious toggle), it's distinctive. Strong fit: Gaming, Maximalist brand sites, Music products.

**Drag-to-explore** — Hero content the user drags around (a floating object, a 3D model, a rotating logo). Strong fit: Maximalist, 3D, Creative portfolio.

**Konami code / hidden interactions** — Easter eggs that reward exploration. Doesn't drive aesthetic alone but adds memorable character. Strong fit: Tech Minimalist, Brutalist (when sites resist polish), Indie.

---

## Typographic Moves

**Variable font axis playground** — A hero typeface that morphs across an axis (weight, width, optical size, stroke contrast) animated continuously or on cursor proximity. Strong fit: Maximalist, Tech-Editorial, Type-driven brand.

**Oversized display crushed against edges** — Hero type at 20vw or larger, with negative margins so it bleeds off the viewport. The composition extends beyond what's visible. Strong fit: Editorial, Brutalist, Maximalist.

**Drop caps on every section** — Each section opens with a 4-line drop cap in the display face. Carries editorial sensibility throughout. Strong fit: Editorial, Literary.

**Pull quotes pulled to the margin** — Quotes set in display italic, optically aligned to the page margin, becoming compositional anchors. Strong fit: Editorial, Long-form.

**Tracked-out caps as section dividers** — `letter-spacing: 0.3em` uppercase headlines as the only ornament. Strong fit: Minimalist, Luxury, Art Deco.

**Numbers as composition** — Issue numbers, dates, page numbers treated as primary typographic elements in condensed/expressive cuts. Strong fit: Editorial, Swiss, Industrial.

**Kinetic type on load** — Display type assembles letter-by-letter, each letter animating in with custom timing. Strong fit: Maximalist, Brand-statement hero.

**Mixed-face composition** — Three typefaces on one page, deliberately clashing, juxtaposed for tension. Strong fit: Lo-Fi, Brutalist, Editorial-rebellious.

**Marquee / ticker** — Horizontal scrolling type loops. The CSS `animation` infinite linear marquee. Strong fit: Brutalist, Maximalist, News/Media.

**Typewriter reveal** — Text appears character-by-character as if typed. Strong fit: Retro-Futurist (terminal), Editorial (long-form opener).

**Variable-axis on scroll** — As user scrolls, a typeface's weight or width morphs (Söhne Variable, Inter Variable). Strong fit: Maximalist, Editorial-Modern.

---

## Layout Motifs

**Asymmetric grid break** — A 12-column grid that breaks intentionally on one section per page — content escapes into the gutter, overlaps with the next module. Strong fit: Editorial, Swiss-modern, Maximalist.

**Full-bleed splits** — Hero sections that divide the viewport into two unequal full-bleed halves (text on one side, image on the other). Strong fit: Editorial, Modern brand sites.

**Floating sticky elements** — A side panel, table of contents, or status indicator that sticks while content scrolls past, with subtle motion responding to scroll position. Strong fit: Editorial, Long-form, Documentation.

**Sectioned color blocks** — Each major section a different full-bleed color, with type and imagery rebalanced per section. Strong fit: Maximalist, Vibrant Block, Editorial.

**Bento grid** — Modular grid of differently-sized cards composing the layout. Strong fit: Tech Minimalist, Modern marketing.

**Edge-to-edge type** — Type runs from the left viewport edge to the right with zero side margin. Strong fit: Brutalist, Editorial, Maximalist hero.

**Diagonal compositions** — Elements aligned along a diagonal axis (45° or other). Strong fit: Maximalist, Memphis Revival, Lo-Fi.

**Z-stack overlap** — Multiple layers (image, type, gradient, shape) overlapping with intentional z-index. Strong fit: Maximalist, Editorial cover sensibility.

**Modular case-study layouts** — Same structural template per case study, varied through content and color. Strong fit: Portfolio, Agency.

**Rule-line marginalia** — Hairline rules and small-caps labels in the page margins, like a printed book. Strong fit: Editorial, Literary, Scholarly.

---

## Texture Treatments

**Film grain overlay** — A `<feTurbulence>` SVG noise layer at 1–4% opacity over the entire viewport. Subtle warmth that's almost unnoticed but adds to feel. Strong fit: Editorial, Organic, Maximalist.

**Halftone photography** — Photos converted to dot patterns via SVG filter or background-image tile. Strong fit: Lo-Fi, Editorial-Punk, Print-inflected.

**Scanlines** — `repeating-linear-gradient` overlay simulating CRT scanlines. Strong fit: Retro-Futurist (CRT, Cyberpunk).

**Paper texture** — Tiled or full-bleed paper-grain image at low opacity, often warm-tinted. Strong fit: Organic, Editorial, Lo-Fi.

**Toner streaks** — Thin vertical lines of slightly lighter color simulating xerox drum wear. Strong fit: Lo-Fi, Brutalist-vintage.

**Mesh gradient hero** — A WebGL or SVG mesh gradient as hero background, animated subtly. Strong fit: Maximalist (Aurora variant), Tech-Modern.

**Noise on glass** — Glassmorphism with added grain on the blurred surface for tactile feel. Strong fit: Maximalist, Tech-Premium.

**Risograph misregister** — Two-color overlays offset by 2–4 pixels, simulating Riso print. Strong fit: Lo-Fi, Editorial-Indie, Print revival.

**Letterpress emboss** — Type appears slightly recessed via inset shadow. Strong fit: Organic, Editorial-Print, Luxury subtle.

**Iridescence / oil-slick** — Multi-stop conic gradients that shift hue across the surface. Strong fit: Maximalist (Liquid Glass variant), Premium Tech.

---

## Material Treatments

**Glassmorphism** — `backdrop-filter: blur()` on semi-transparent surfaces. The 2020s tentpole material. Strong fit: Maximalist, Tech-Modern, iOS-influenced.

**Claymorphism** — Soft 3D-ish surfaces with double shadows (inner highlight + outer drop). Strong fit: Maximalist (playful), Education K-12, Children's products.

**Skeuomorphism (selective)** — Realistic textures on key surfaces (leather, paper, wood) deployed sparingly. Strong fit: Premium consumer, Hospitality, period-appropriate.

**Liquid glass / morphing** — SVG-morphing surfaces with chromatic aberration. Strong fit: Maximalist (Liquid variant), Premium Apple-VisionOS-adjacent.

**Hard offset shadows** — `box-shadow: 8px 8px 0 #000`, no blur. Strong fit: Brutalist (neo), Vibrant Block, Maximalist-Memphis.

**Soft layered shadows** — Multi-stop `box-shadow` with varied blur and spread. Strong fit: Minimalist, Tech-Premium, Refined.

**Chrome / metallic surfaces** — SVG gradient fills simulating chrome. Strong fit: Retro-Futurist (Y2K, Atompunk), Art Deco, Premium.

**3D objects in WebGL** — Three.js / Spline objects rendered live in the viewport. Strong fit: Maximalist (3D variant), Brand experience, Product demo.

---

## Color Anchors

**Single-ink composition** — Entire site in two colors: surface and one ink. The accent appears at most 2–3 times per page. Strong fit: Editorial, Minimalist, Lo-Fi.

**Domain-derived palette** — Palette pulled directly from product subject matter (food brand from ingredient colors, outdoor brand from landscape photography). Strong fit: Organic, Brand-storytelling.

**Forced duotone photography** — All photography rendered in two colors (often the brand colors). Strong fit: Editorial, Maximalist, Lo-Fi.

**Color section per chapter** — Each major section has its own palette; the whole site is a journey through color. Strong fit: Maximalist, Editorial-narrative.

**Monochromatic with one neon** — Greyscale composition with one full-saturation neon accent. Strong fit: Industrial, Tech Minimalist, Cyberpunk-light.

**Gradient as identity** — A signature multi-stop gradient that appears on key surfaces (hero, primary buttons, brand mark). Strong fit: Maximalist (Aurora), Tech-Modern.

**Inverted dark mode** — Dark mode that's not desaturated but shifted entirely (e.g., warm sunset for "night," cool dawn for "day"). Strong fit: Reading apps, Mood-keyed brands.

---

## Motion Signatures

**Spring-physics primary motion** — All transitions use spring physics rather than cubic-bezier. The product feels material. Strong fit: Maximalist, Apple-adjacent, Tech-Premium.

**Stagger-on-load orchestration** — Hero elements appear in choreographed sequence with deliberate timing. Strong fit: Editorial, Maximalist, Brand-statement.

**Scroll-linked parallax (subtle)** — Background and foreground move at different rates. Strong fit: Editorial, Maximalist, Storytelling.

**Page transitions as full-bleed motion** — Navigating between pages triggers a full-page reveal (slide, wipe, color flood). Strong fit: Maximalist, Brand-experience, Portfolio.

**Shared element transitions** — A clicked card morphs into the destination page's hero. Strong fit: Tech Minimalist, Native-app-inspired web.

**Ambient idle motion** — Subtle continuous animation when nothing is happening (slow gradient drift, breathing scale, soft particle drift). Strong fit: Maximalist, Brand sites, Premium.

**Snap motion (zero ease)** — All transitions instant, no smoothing. The product feels confrontational. Strong fit: Brutalist, Lo-Fi, Tech-utilitarian.

**Type kinetics** — Display type animates on viewport entry — letters scale, weight shifts, characters morph. Strong fit: Maximalist, Brand-statement, Type-led design.

**Cursor-driven 3D tilt** — Hero elements tilt subtly toward the cursor (`transform: rotateX/rotateY` based on mouse position). Strong fit: Maximalist, 3D, Premium product hero.

---

## Data Visualization Moves

**Sparklines as inline type** — Tiny charts inset into prose where a number is mentioned. Strong fit: Editorial-data, Industrial, Modern news.

**Live-updating numerics** — Numbers ticking up/down with tabular precision in real-time. Strong fit: Industrial, Financial, Music streaming.

**Custom chart aesthetic** — Charts that match the brand's typography, color, motion language — not generic Chart.js defaults. Strong fit: Industrial, Editorial-data, Premium.

**Annotated charts** — Inline annotations, callouts, and marginalia on charts (NYT Upshot style). Strong fit: Editorial-journalism, Industrial, Storytelling.

**Color-coded heatmaps** — Surfaces where color encodes data density. Strong fit: Industrial (analytics), Map products.

---

## How to Pick

For a given project: read the differentiator categories above and pick *one* anchor that:
1. Reinforces the chosen archetype (organic projects pull organic signatures; brutalist projects pull brutalist signatures)
2. The audience would remember after leaving
3. You can implement well within scope (not a half-built version)

If you can name three anchors but only commit to one, name the chosen one in the differentiator step of the operating mode. The other two are fine inspiration but stay off the page.
