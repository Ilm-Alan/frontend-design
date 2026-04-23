# Palettes by Mood

When the product domain is unclear, ambiguous, or you want a feeling-first palette rather than a category-first one, pull from these mood-keyed palettes. Each is a complete starting point — primary surface, foreground, accent, supporting tones.

---

## Trust (cool blue, restrained)

For: financial, healthcare, B2B, governance, anywhere "we will not betray you" is the message.

```css
--surface: #F8FAFC;
--foreground: #0F172A;
--primary: #1E40AF;
--accent: #0369A1;
--muted: #E2E8F0;
--border: #CBD5E1;
```

Tone variations: warmer toward navy + parchment for established/old-money trust; cooler toward steel-blue for tech-forward trust.

---

## Luxury (deep + metallic)

For: premium retail, hospitality, fashion, fragrance, spirits.

```css
--surface: #FAFAF9;             /* light variant */
--foreground: #0C0A09;
--primary: #1C1917;
--accent: #A16207;              /* aged gold */
--muted: #E7E5E4;
```

Dark variant (often the preferred mode):
```css
--surface: #0A0908;
--foreground: #F4F1EC;
--primary: #F4F1EC;
--accent: #C9A96E;              /* lit gold against dark */
```

Gold appears as borders, hairlines, monograms. Fill colors come from other surfaces.

---

## Refined (ivory + ink + one muted accent)

For: editorial, literary, considered consumer products, design portfolios.

```css
--surface: #F8F4EC;             /* ivory */
--foreground: #1A1714;          /* warm ink */
--accent: #4A1F3A;              /* deep aubergine */
--muted: #EFE9DD;
--border: #DDD2BD;
```

Swap accent for: brick `#9A3B2E`, navy `#1A2F4A`, oxblood `#5C1A1A`, sage `#5E6F58`, ochre `#C08E3A` — pick one and live with it.

---

## Playful (saturated primaries)

For: children's products, casual games, consumer mobile apps, education K-12.

```css
--surface: #FEFEFE;
--foreground: #1A1A2E;
--primary: #4F46E5;             /* indigo */
--secondary: #FBBF24;           /* yellow */
--accent: #EA580C;              /* orange */
--success: #22C55E;
```

The trick: 60/30/10 dominance with primaries — without that ratio, playful collapses into chaos.

---

## Energetic (neon, vibrant)

For: fitness, gaming, music, youth-oriented brands, creative tools.

```css
--surface: #0A0A0F;
--foreground: #F8FAFC;
--primary: #FF006E;             /* hot pink */
--secondary: #3A86FF;           /* electric blue */
--accent: #FFEE00;              /* acid yellow */
--muted: #1A1A24;
```

Light variant inverts the surface but keeps neon saturation. Glow effects (`text-shadow: 0 0 20px ...`) reinforce the energy.

---

## Calm (desaturated cool)

For: meditation, sleep, journaling, productivity tools that aim to keep the user at ease.

```css
--surface: #F0F4F8;
--foreground: #2A3D4F;
--primary: #5B7C99;             /* dusty steel-blue */
--accent: #8FA8B5;              /* lighter blue-grey */
--muted: #DCE3EA;
```

Saturation throughout stays low. No accent jumps above 30% saturation. Shadows soft and shallow.

---

## Urgent (red/orange/black)

For: emergency, breaking news, sale moments, alert systems, single-use urgency.

```css
--surface: #0A0A0A;
--foreground: #FFFFFF;
--primary: #DC2626;             /* alarm red */
--accent: #FF6B00;              /* burning orange */
--warning: #FBBF24;
```

Use sparingly — entire-product urgency palettes burn out the user. Better deployed in modals, banners, single sections.

---

## Natural (earth tones)

For: organic products, farm-to-table, craft brands, outdoor gear, sustainability-forward.

```css
--surface: #F8F4EC;             /* cream */
--foreground: #2D2419;          /* warm earth-black */
--primary: #606C38;             /* moss */
--secondary: #B08B6E;           /* clay */
--accent: #C66B3D;              /* terracotta */
--muted: #E8DCC7;               /* sand */
```

All tones share warmth — no cool greys, no pure whites, no pure blacks.

---

## Retro 80s (synthwave)

For: products evoking 1980s aesthetic — synthwave, Miami Vice, retro-cool.

```css
--surface: #0F0E17;             /* deep navy near-black */
--foreground: #FAFAFA;
--primary: #FF006E;             /* hot pink */
--secondary: #8338EC;           /* purple */
--accent: #FB5607;              /* orange */
--muted: #FFBE0B;               /* yellow highlight */
```

Background often gradients from `#FF006E` → `#8338EC` → `#FB5607` for hero sections. Wireframe horizons in `#FFBE0B`.

---

## Futurist (neon on deep)

For: cyberpunk, sci-fi adjacent, tech brands wanting "future" not "present."

```css
--surface: #0A0014;             /* deep dark */
--foreground: #E0E0E0;
--primary: #00FFAB;             /* mint neon */
--secondary: #3A86FF;           /* electric blue */
--accent: #FF006E;              /* magenta */
```

Add `text-shadow: 0 0 8px var(--color-primary)` to accent type for bloom. Chromatic aberration optional.

---

## Noir (monochrome + one ink)

For: serious editorial, single-creator portfolios, photography sites, anything that wants restraint with personality.

```css
--surface: #FAFAFA;
--foreground: #0A0A0A;
--primary: #0A0A0A;
--accent: #DC2626;              /* one ink — swap for any single saturated color */
--muted: #E5E5E5;
--border: #D4D4D4;
```

The accent appears two or three times per page. The composition does the work.

---

## Warm Professional (warm neutrals + navy)

For: legal, financial advisors, hospitality, established consultancies.

```css
--surface: #F5F2EC;             /* warm parchment */
--foreground: #1A2238;          /* navy */
--primary: #1A2238;
--accent: #A47148;              /* warm camel */
--muted: #E5DCC8;
```

Bridges luxury and corporate — feels established without feeling corporate.

---

## Bold Editorial (ivory + ink + saturated accent)

For: arts publications, fashion editorial digital, modern magazines.

```css
--surface: #F8F4EC;
--foreground: #0E0D0B;
--primary: #0E0D0B;
--accent: #FF3D2E;              /* signal red */
--muted: #EFE9DD;
```

The accent is dramatic — used in pull quotes, signature elements, single CTAs. The contrast against ivory is the move.

---

## Cyberpunk (neon green/magenta + pitch black)

For: gritty future, hacker aesthetic, technical-creative tools wanting edge.

```css
--surface: #000000;
--foreground: #00FF41;          /* terminal green */
--primary: #FF006E;             /* magenta */
--accent: #00FFFF;              /* cyan */
--muted: #1A1A1A;
```

Monospace dominant. Glitch effects appropriate. Scanline overlay reinforces the mood.

---

## Pastel (soft tints + one saturated pop)

For: lifestyle brands, contemporary wellness, design-conscious consumer.

```css
--surface: #FFF8F3;             /* peach cream */
--foreground: #2D2A26;
--primary: #FFB5A7;             /* peach */
--secondary: #C9E4DE;           /* soft mint */
--accent: #E63946;              /* one saturated pop */
--muted: #F1E8E0;
```

Pastels alone read childish; the one saturated accent grants seriousness.

---

## How to choose a mood

If the project brief named an emotional register ("calm," "premium," "energetic"), use that. If not, ask: *what's the one feeling someone should have when they land on this?* The mood that answers it is the palette.

If two moods both feel right, the product probably needs to choose. Indecision in mood reads as indecision in design.
