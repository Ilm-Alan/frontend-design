# Palettes by Product Domain

Distilled, semantic-token-ready palettes keyed to product type. Use these as starting points; tune the accent and mood within each archetype's vocabulary. Each entry follows the shadcn semantic token pattern (`primary`, `secondary`, `accent`, `surface`, `foreground`, `card`, `muted`, `border`, `destructive`, `ring`).

When in doubt, pull from the closest domain and shift the accent toward the brand's emotional register.

---

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
