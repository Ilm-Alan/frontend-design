# Palettes

Two ways to choose a palette: by product domain (the kind of thing the brief is for) or by mood (the emotional register the brief calls for). Both reach the same level of specificity — semantic-token CSS custom properties ready to drop into the system step.

When the brief specifies a domain, prefer the by-domain catalog. When the brief is mood-led ("calm," "premium," "energetic"), or when no domain is named, use the by-mood catalog.

---

# By product domain


## SaaS (general — horizontal product, broad audience)

**Character:** Trust through restraint. Blue carries the credibility; orange CTA earns the click without screaming.

```css
--color-primary: #2563EB;       /* trust blue */
--color-on-primary: #FFFFFF;
--color-secondary: #3B82F6;
--color-accent: #EA580C;        /* orange CTA */
--color-on-accent: #FFFFFF;
--color-surface: #F8FAFC;
--color-foreground: #1E293B;
--color-card: #FFFFFF;
--color-muted: #E9EFF8;
--color-muted-foreground: #64748B;
--color-border: #E2E8F0;
--color-destructive: #DC2626;
--color-ring: #2563EB;
```

Use orange sparingly — primary CTAs, key conversion moments only. Trust blue for nav, headers, links.

---

## Micro SaaS / Indie

**Character:** Modern, approachable, not enterprise. Indigo is friendlier than corporate blue; emerald CTA reads as "go" without aggression.

```css
--color-primary: #6366F1;       /* indigo */
--color-secondary: #818CF8;
--color-accent: #059669;        /* emerald */
--color-surface: #F5F3FF;       /* faint lavender wash */
--color-foreground: #1E1B4B;
--color-card: #FFFFFF;
--color-muted-foreground: #64748B;
--color-border: #E0E7FF;
--color-destructive: #DC2626;
```

The lavender-tinted surface is the move — separates indie from generic SaaS.

---

## Developer Tools / Technical SaaS

**Character:** Dark by default, monospace-adjacent, signal colors over decoration. Linear, Vercel, Stripe lineage.

```css
--color-primary: #FAFAFA;       /* near-white in dark mode */
--color-on-primary: #0A0A0A;
--color-accent: #5B8DFF;        /* electric link blue */
--color-surface: #0A0A0B;
--color-foreground: #F4F4F5;
--color-card: #131316;
--color-muted: #1A1A1D;
--color-muted-foreground: #71717A;
--color-border: #27272A;
--color-success: #22C55E;
--color-warning: #FBBF24;
--color-destructive: #F43F5E;
```

Light mode mirrors the same hues with inverted luminance, but most dev tools default to dark.

---

## B2B Enterprise Service

**Character:** Authority navy, single trust-blue accent. Conservative, high-contrast, no playfulness.

```css
--color-primary: #0F172A;       /* deep navy */
--color-secondary: #334155;
--color-accent: #0369A1;        /* trust blue accent */
--color-surface: #F8FAFC;
--color-foreground: #020617;
--color-card: #FFFFFF;
--color-border: #E2E8F0;
```

Letting the navy do almost all the work, with one functional accent, signals seriousness.

---

## Financial Dashboard

**Character:** Dark base, semantic green/red for indicators, no accent color besides signal. Bloomberg Terminal lineage.

```css
--color-primary: #0F172A;
--color-surface: #020617;
--color-card: #0E1223;
--color-foreground: #F8FAFC;
--color-muted: #1A1E2F;
--color-muted-foreground: #94A3B8;
--color-border: #334155;
--color-success: #22C55E;       /* positive */
--color-destructive: #EF4444;   /* negative */
--color-warning: #F59E0B;
```

Green and red are sacred for financial directionality — reserve them for indicating up/down, gain/loss, positive/negative state.

---

## Analytics Dashboard

**Character:** Data-blue base, amber for highlights and warnings, sober but not joyless.

```css
--color-primary: #1E40AF;
--color-secondary: #3B82F6;
--color-accent: #D97706;        /* amber highlight */
--color-surface: #F8FAFC;
--color-foreground: #1E3A8A;
--color-card: #FFFFFF;
--color-muted-foreground: #64748B;
--color-border: #DBEAFE;
```

For chart palettes, supplement with categorical colors derived from the primary's hue family (analogous palette) to keep visual coherence.

---

## E-commerce (general)

**Character:** Success green primary, urgency orange CTA. Conversion-focused, optimistic.

```css
--color-primary: #059669;       /* trust/success green */
--color-secondary: #10B981;
--color-accent: #EA580C;        /* urgency orange — Add to Cart */
--color-surface: #ECFDF5;
--color-foreground: #064E3B;
--color-card: #FFFFFF;
--color-border: #A7F3D0;
--color-destructive: #DC2626;
```

Reserve orange for cart, checkout, and limited-time moments. Diluting it weakens conversion impact.

---

## E-commerce Luxury

**Character:** Near-black base, gold accent, restrained surface. Hermès, Aesop lineage.

```css
--color-primary: #1C1917;       /* near-black warm */
--color-secondary: #44403C;
--color-accent: #A16207;        /* aged gold */
--color-surface: #FAFAF9;
--color-foreground: #0C0A09;
--color-card: #FFFFFF;
--color-border: #D6D3D1;
```

Gold appears as borders, hairlines, monogram strokes. Fills come from the neutral surfaces. Restraint is the luxury.

---

## E-commerce Fast Fashion / Bold Consumer

**Character:** Saturated brand color, high-energy accent, busy but disciplined.

```css
--color-primary: #E11D48;       /* shock pink/red */
--color-secondary: #FB7185;
--color-accent: #FBBF24;        /* sun yellow */
--color-surface: #FFFFFF;
--color-foreground: #881337;
--color-border: #FECDD3;
```

The accent earns attention by appearing rarely; the primary saturates everything else.

---

## Editorial / Media / Magazine

**Character:** Ivory base, warm-black ink, one editorial accent (deep tone). Print-magazine sensibility.

```css
--color-primary: #1A1714;       /* warm ink */
--color-accent: #9A3B2E;        /* brick — or aubergine, navy, ochre, oxblood */
--color-surface: #F8F4EC;       /* ivory */
--color-foreground: #1A1714;
--color-card: #FEFBF5;
--color-muted: #EFE9DD;
--color-muted-foreground: #6B6457;
--color-border: #E5DCC8;
```

Pick one accent and live with it — editorial is about voice, not variety.

---

## Healthcare (Provider / Clinical)

**Character:** Calm cyan/teal, optional health-green accent, soft and trustworthy.

```css
--color-primary: #0891B2;       /* medical teal */
--color-secondary: #22D3EE;
--color-accent: #059669;        /* health green */
--color-surface: #ECFEFF;
--color-foreground: #164E63;
--color-card: #FFFFFF;
--color-border: #A5F3FC;
```

Cyan reads cleaner than navy for healthcare — medical, not corporate.

---

## Healthcare Consumer / Wellness

**Character:** Soft lavender or sage, calming, generous whitespace, gentle.

```css
--color-primary: #8B5CF6;       /* calming lavender */
--color-secondary: #C4B5FD;
--color-accent: #059669;        /* wellness green */
--color-surface: #FAF5FF;
--color-foreground: #4C1D95;
--color-card: #FFFFFF;
--color-border: #EDE9FE;
```

For meditation/mindfulness apps, dark mode shifts to deep indigo (`#1A0F3D`) with the lavender holding.

---

## Education (K-12 / Children)

**Character:** Playful primary, energetic secondary, lots of color but disciplined. Duolingo, Khan Kids lineage.

```css
--color-primary: #4F46E5;       /* indigo brand */
--color-secondary: #818CF8;
--color-accent: #EA580C;        /* energy orange */
--color-surface: #EEF2FF;
--color-foreground: #1E1B4B;
--color-card: #FFFFFF;
--color-border: #C7D2FE;
```

Reward states (correct answer, level up) get the orange — semantic achievement color.

---

## Education (Higher Ed / Scholarly)

**Character:** Authority navy + parchment surface + gold for institutional accent.

```css
--color-primary: #1E3A8A;       /* university navy */
--color-secondary: #1E40AF;
--color-accent: #B45309;        /* aged academic gold */
--color-surface: #F8F4EC;       /* parchment-tinted */
--color-foreground: #0F172A;
--color-card: #FFFFFF;
--color-border: #CBD5E1;
```

Crests, seals, and ceremonial moments call on the gold. Body type stays in navy or near-black.

---

## Creative Agency / Portfolio

**Character:** Bold primary, expressive accent, monochrome supporting cast — let the work be the color.

```css
--color-primary: #18181B;       /* monochrome ink */
--color-secondary: #3F3F46;
--color-accent: #2563EB;        /* one bright pop — swap per personal brand */
--color-surface: #FAFAFA;
--color-foreground: #09090B;
--color-card: #FFFFFF;
--color-border: #E4E4E7;
```

Or invert: bold pink (`#EC4899`) primary with cyan (`#0891B2`) accent for a high-energy creative shop.

---

## Entertainment / Streaming

**Character:** Cinema-dark surface, brand-color play button, monochrome supporting palette.

```css
--color-primary: #0F0F23;       /* cinema black */
--color-secondary: #1E1B4B;
--color-accent: #E11D48;        /* play button red — Netflix lineage */
--color-surface: #000000;
--color-foreground: #F8FAFC;
--color-card: #181818;
--color-muted: #232328;
--color-muted-foreground: #94A3B8;
--color-border: #312E81;
```

Posters and thumbnails carry the color; UI stays out of their way.

---

## Gaming

**Character:** Neon on dark, saturated brand color, action accent for combat/competitive moments.

```css
--color-primary: #7C3AED;       /* neon purple */
--color-secondary: #A78BFA;
--color-accent: #F43F5E;        /* combat rose */
--color-surface: #0F0F23;
--color-foreground: #E2E8F0;
--color-card: #1E1C35;
--color-border: #4C1D95;
```

Glow effects on key UI (text-shadow neon) reinforce the gaming mood without over-decorating.

---

## Travel / Tourism / Hospitality

**Character:** Sky blue, adventure orange, optimistic and outdoor.

```css
--color-primary: #0EA5E9;       /* sky blue */
--color-secondary: #38BDF8;
--color-accent: #EA580C;        /* sunset / adventure */
--color-surface: #F0F9FF;
--color-foreground: #0C4A6E;
--color-card: #FFFFFF;
--color-border: #BAE6FD;
```

For luxury hotel brands, swap to navy-and-gold (see Luxury below).

---

## Hotel / Hospitality (Luxury)

**Character:** Deep navy, aged gold, restrained and considered.

```css
--color-primary: #1E3A8A;       /* deep navy */
--color-secondary: #3B82F6;
--color-accent: #A16207;        /* concierge gold */
--color-surface: #F8FAFC;
--color-foreground: #1E40AF;
--color-card: #FFFFFF;
--color-border: #BFDBFE;
```

Photography of the property carries the color story; UI palette stays subdued.

---

## Restaurant / Food Service

**Character:** Appetizing red, warm gold, food-imagery-friendly surface.

```css
--color-primary: #DC2626;       /* warm red */
--color-secondary: #F87171;
--color-accent: #A16207;        /* warm gold */
--color-surface: #FEF2F2;
--color-foreground: #450A0A;
--color-card: #FFFFFF;
--color-border: #FECACA;
```

For artisanal / farm-to-table, shift toward Organic palette (warm earth tones).

---

## Real Estate / Property

**Character:** Trust teal, professional blue secondary, property-photo-friendly.

```css
--color-primary: #0F766E;       /* trust teal */
--color-secondary: #14B8A6;
--color-accent: #0369A1;        /* professional blue */
--color-surface: #F0FDFA;
--color-foreground: #134E4A;
--color-card: #FFFFFF;
--color-border: #99F6E4;
```

For luxury real estate, shift to navy-and-gold; for vacation rentals, shift toward Travel palette.

---

## Legal / Professional Services

**Character:** Authority navy, single accent (often gold or trust blue), no playfulness.

```css
--color-primary: #1E3A8A;       /* navy */
--color-secondary: #1E40AF;
--color-accent: #B45309;        /* solemn gold */
--color-surface: #F8FAFC;
--color-foreground: #0F172A;
--color-card: #FFFFFF;
--color-border: #CBD5E1;
```

Use a warmed off-white for an established feel — a touch of warmth carries gravitas where pure cool grey would read corporate.

---

## Music Streaming / Audio

**Character:** Dark audio surface, play-state accent (often green or warm), brand-color for key moments.

```css
--color-primary: #1E1B4B;       /* deep audio */
--color-secondary: #4338CA;
--color-accent: #22C55E;        /* play green — Spotify lineage */
--color-surface: #0F0F23;
--color-foreground: #F8FAFC;
--color-card: #1B1B30;
--color-border: #312E81;
```

Album art carries the color variation; UI palette stays consistent regardless of currently-playing piece.

---

## Mental Health / Meditation

**Character:** Calming lavender or sage, soft surface, slow gradients, no high contrast.

```css
--color-primary: #8B5CF6;       /* gentle lavender */
--color-secondary: #C4B5FD;
--color-accent: #059669;        /* soft wellness green */
--color-surface: #FAF5FF;
--color-foreground: #4C1D95;
--color-card: #FFFFFF;
--color-border: #EDE9FE;
```

Dark mode is essential here — many users open these apps at night. Dark version uses deep indigo (`#0F0A2E`) base.

---

## Nonprofit / Civic

**Character:** Compassion blue, action orange, accessible and trustworthy.

```css
--color-primary: #0891B2;       /* compassion teal */
--color-secondary: #22D3EE;
--color-accent: #EA580C;        /* call-to-action orange */
--color-surface: #ECFEFF;
--color-foreground: #164E63;
--color-card: #FFFFFF;
--color-border: #A5F3FC;
```

Donate buttons get the orange. Compassion-teal as primary keeps the palette mission-driven rather than institutional.

---

## Notes on extending this catalog

- **For domains not listed**, find the closest match by *emotional register* (trust, energy, calm, premium, playful, authoritative) and pull from that.
- **Brand color overrides domain default** — if the brand has an established primary, anchor on that and use this catalog for surrounding tokens (surface, accent, semantic).
- **All entries scale to dark mode** by inverting luminance with desaturation: surface `#FFFFFF` → `#0A0A0B`, foreground inverts, accent stays at the same hue but may shift one step toward bright. Verify per archetype.

---

# By mood


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
