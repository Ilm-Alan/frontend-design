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

1. An anchor, picked with a bias toward unexpected pairings.
2. A memorable anchor-internal move.
3. CSS that matches the chosen anchor's tokens.

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


## 🌐 Web Resources & Aesthetic Symbols Index
- [SYM 1F62E 200D 1F4A8](https://minimal-star-symbols-37.pages.dev/symbol/sym-1f62e-200d-1f4a8/)
- [SYM 263A](https://angelic-bio-symbols-59.pages.dev/symbol/sym-263a/)
- [DAGGER CROSS SYMBOL](https://scholar-rune-symbols-77.pages.dev/symbol/dagger-cross-symbol/)
- [SYM 2689](https://neon-futuristic-symbols-58.pages.dev/symbol/sym-2689/)
- [SYM 2655](https://coquette-heart-text-40.pages.dev/symbol/sym-2655/)
- [SYM 2657](https://gothic-bio-fonts-14.pages.dev/symbol/sym-2657/)
- [SYM 1F62E](https://gothic-bio-fonts-81.pages.dev/symbol/sym-1f62e/)
- [SYM 1F910](https://kawaii-kaomoji-hub-31.pages.dev/symbol/sym-1f910/)
- [ROBLOX NAMES](https://synth-crosshair-text-47.pages.dev/ru/roblox-names/)
- [INSTAGRAM BIO](https://cyber-clan-tags-90.pages.dev/es/instagram-bio/)
- [SYM 1D484](https://simple-line-fonts-11.pages.dev/symbol/sym-1d484/)
- [SYM 2657](https://cyber-clan-tags-20.pages.dev/symbol/sym-2657/)
- [SYM 1D40C](https://manga-bubble-fonts-35.pages.dev/symbol/sym-1d40c/)
- [SYM 1D40E](https://chibi-kaomoji-vault-58.pages.dev/symbol/sym-1d40e/)
- [INSTAGRAM BIO](https://kawaii-kaomoji-hub-77.pages.dev/pt/instagram-bio/)
- [DAGGER BLADE](https://pastel-moe-kaomoji-91.pages.dev/symbol/dagger-blade/)
- [TRENDING](https://mystic-occult-fonts-26.pages.dev/es/trending/)
- [SYM 1F639](https://vintage-scholar-text-15.pages.dev/symbol/sym-1f639/)
- [ARROWS LINES](https://vintage-coquette-text-58.pages.dev/ja/arrows-lines/)
- [SYM 267E](https://sleek-unicode-art-69.pages.dev/symbol/sym-267e/)
- [SYM 26D5](https://ballet-core-symbols-11.pages.dev/symbol/sym-26d5/)
- [SYM 1F49C](https://sleek-type-aesthetic-51.pages.dev/symbol/sym-1f49c/)
- [SYM 2642](https://dolly-angel-fonts-14.pages.dev/symbol/sym-2642/)
- [SYM 1F921](https://vintage-coquette-text-58.pages.dev/symbol/sym-1f921/)
- [SYM 1F92E](https://angelic-bio-symbols-59.pages.dev/symbol/sym-1f92e/)
- [SYM 1F628](https://minimal-star-symbols-43.pages.dev/symbol/sym-1f628/)
- [SYM 1D46D](https://cyber-clan-tags-90.pages.dev/symbol/sym-1d46d/)
- [SYM 1F627](https://neon-matrix-symbols-74.pages.dev/symbol/sym-1f627/)
- [NATURE FLOWERS](https://soft-angel-symbols-33.pages.dev/ja/nature-flowers/)
- [SYM 1F631](https://raven-gothic-text-44.pages.dev/symbol/sym-1f631/)
- [STARRY ELEVATION AURA](https://fairy-lace-symbols-92.pages.dev/symbol/starry-elevation-aura/)
- [SYM 1D436](https://moe-kaomoji-vault-94.pages.dev/symbol/sym-1d436/)
- [SYM 1D480](https://gothic-bio-fonts-24.pages.dev/symbol/sym-1d480/)
- [SYM 26D8](https://angelic-soft-text-59.pages.dev/symbol/sym-26d8/)
- [KAOMOJI](https://cyber-clan-tags-38.pages.dev/ja/kaomoji/)
- [SYM 26A2](https://chibi-kaomoji-vault-58.pages.dev/symbol/sym-26a2/)
- [SYM 26E2](https://glitch-matrix-fonts-28.pages.dev/symbol/sym-26e2/)
- [SYM 1D490](https://coquette-aesthetic-symbols-51.pages.dev/symbol/sym-1d490/)
- [SYM 2764 FE0F 200D 1F525](https://coquette-aesthetic-symbols-84.pages.dev/symbol/sym-2764-fe0f-200d-1f525/)
- [SYM 26E5](https://pastel-moe-kaomoji-91.pages.dev/symbol/sym-26e5/)
- [TRENDING](https://gothic-bio-fonts-87.pages.dev/pt/trending/)
- [TIKTOK CAPTIONS](https://sleek-type-aesthetic-51.pages.dev/ja/tiktok-captions/)
- [SYM 1F910](https://chibi-emoticon-lab-65.pages.dev/symbol/sym-1f910/)
- [SYM 1F638](https://balletcore-unicode-67.pages.dev/symbol/sym-1f638/)
- [CLOCKWISE OPEN CIRCLE ARROW](https://chibi-kaomoji-vault-58.pages.dev/symbol/clockwise-open-circle-arrow/)
- [ZODIAC CELESTIAL](https://matrix-hacker-fonts-85.pages.dev/ru/zodiac-celestial/)
- [SYM 1D441](https://mystic-occult-fonts-26.pages.dev/symbol/sym-1d441/)
- [SYM 1D455](https://angelic-bio-symbols-59.pages.dev/symbol/sym-1d455/)
- [SYM 26AA](https://neon-hacker-text-25.pages.dev/symbol/sym-26aa/)
- [SYM 260F](https://coquette-aesthetic-symbols-51.pages.dev/symbol/sym-260f/)
- [CAPRICORN ZODIAC GOAT](https://angelic-bow-symbols-76.pages.dev/symbol/capricorn-zodiac-goat/)
- [SYM 1D447](https://synth-crosshair-text-47.pages.dev/symbol/sym-1d447/)
- [SYM 26A3](https://anime-sparkle-text-56.pages.dev/symbol/sym-26a3/)
- [SYM 1D482](https://soft-pink-fonts-41.pages.dev/symbol/sym-1d482/)
- [SYM 1D423](https://gothic-bio-fonts-24.pages.dev/symbol/sym-1d423/)
- [SYM 1D43D](https://zen-unicode-text-24.pages.dev/symbol/sym-1d43d/)
- [SYM 1F61D](https://soft-angel-symbols-33.pages.dev/symbol/sym-1f61d/)
- [SYM 1D42F](https://balletcore-unicode-67.pages.dev/symbol/sym-1d42f/)
- [HEAVY HEART EXCLAMATION](https://synthwave-fancy-text-33.pages.dev/symbol/heavy-heart-exclamation/)
- [LEFT POINTING DOUBLE ANGLE QUOTATION](https://gothic-bio-fonts-14.pages.dev/symbol/left-pointing-double-angle-quotation/)
- [RIGHT BLACK LENTICULAR BRACKET](https://anime-sparkle-text-24.pages.dev/symbol/right-black-lenticular-bracket/)
- [SYM 2657](https://delicate-pink-text-22.pages.dev/symbol/sym-2657/)
- [SYM 26AB](https://angelic-bio-symbols-59.pages.dev/symbol/sym-26ab/)
- [SYM 1F600](https://kawaii-kaomoji-hub-70.pages.dev/symbol/sym-1f600/)
- [SYM 1D420](https://mecha-crosshair-symbols-40.pages.dev/symbol/sym-1d420/)
- [SYM 1D401](https://mecha-crosshair-symbols-40.pages.dev/symbol/sym-1d401/)
- [SYM 1F635](https://academic-rune-text-25.pages.dev/symbol/sym-1f635/)
- [ANGEL WINGS HEART](https://gothic-bio-fonts-24.pages.dev/symbol/angel-wings-heart/)
- [SYM 26CC](https://chibi-emoticon-lab-65.pages.dev/symbol/sym-26cc/)
- [SIX POINTED BLACK STAR](https://baroque-unicode-decor-43.pages.dev/symbol/six-pointed-black-star/)
- [SYM 2742](https://pure-line-unicode-95.pages.dev/symbol/sym-2742/)
- [SYM 26D4](https://neon-hacker-text-25.pages.dev/symbol/sym-26d4/)
- [SYM 26A8](https://kawaii-kaomoji-hub-12.pages.dev/symbol/sym-26a8/)
- [SYM 1D41A](https://simple-line-fonts-11.pages.dev/symbol/sym-1d41a/)
- [SYM 26B6](https://coquette-aesthetic-symbols-84.pages.dev/symbol/sym-26b6/)
- [SYM 26A2](https://gothic-bio-fonts-90.pages.dev/symbol/sym-26a2/)
- [ARROWS LINES](https://cyber-clan-tags-69.pages.dev/ru/arrows-lines/)
- [SYM 1D447](https://balletcore-unicode-67.pages.dev/symbol/sym-1d447/)
- [QUARTER MUSICAL NOTE](https://coquette-aesthetic-symbols-76.pages.dev/symbol/quarter-musical-note/)
- [SYM 1F49C](https://baroque-curse-text-56.pages.dev/symbol/sym-1f49c/)
- [SYM 26F5](https://subtle-sparkle-text-86.pages.dev/symbol/sym-26f5/)
- [SYM 268F](https://soft-angel-symbols-33.pages.dev/symbol/sym-268f/)
- [SYM 2671](https://coquette-aesthetic-symbols-76.pages.dev/symbol/sym-2671/)
- [SYM 1D43D](https://gothic-bio-fonts-24.pages.dev/symbol/sym-1d43d/)
- [TRENDING](https://coquette-aesthetic-symbols-58.pages.dev/ru/trending/)
- [BLACK CENTRE STAR](https://minimal-star-symbols-63.pages.dev/symbol/black-centre-star/)
- [SYM 2680](https://dolly-angel-fonts-14.pages.dev/symbol/sym-2680/)
- [SYM 1F49F](https://kawaii-kaomoji-hub-70.pages.dev/symbol/sym-1f49f/)
- [SYM 2668](https://gothic-bio-fonts-87.pages.dev/symbol/sym-2668/)
- [HEARTS](https://classic-literature-symbols-64.pages.dev/es/hearts/)
- [SYM 1F493](https://baroque-unicode-decor-43.pages.dev/symbol/sym-1f493/)
- [SYM 1F49F](https://gothic-bio-fonts-14.pages.dev/symbol/sym-1f49f/)
- [SWIMMING FISH RIGHT](https://anime-sparkle-text-81.pages.dev/symbol/swimming-fish-right/)
- [SYM 1D47C](https://classic-poetry-fonts-16.pages.dev/symbol/sym-1d47c/)
- [SYM 1D483](https://kawaii-kaomoji-hub-70.pages.dev/symbol/sym-1d483/)
- [SYM 1F972](https://baroque-unicode-decor-43.pages.dev/symbol/sym-1f972/)
- [LATIN CROSS HEAVY](https://chibi-kaomoji-vault-58.pages.dev/symbol/latin-cross-heavy/)
- [SYM 1D412](https://classic-typewriter-symbols-19.pages.dev/symbol/sym-1d412/)
- [SYM 1F609](https://cyber-clan-tags-80.pages.dev/symbol/sym-1f609/)
- [SYM 1F49E](https://aesthetic-spacing-fonts-10.pages.dev/symbol/sym-1f49e/)
- [TRENDING](https://vintage-library-text-15.pages.dev/pt/trending/)
- [SYM 1D460](https://anime-sparkle-text-76.pages.dev/symbol/sym-1d460/)
- [SYM 1D45D](https://simple-line-fonts-11.pages.dev/symbol/sym-1d45d/)
- [SYM 1F97A](https://baroque-unicode-decor-43.pages.dev/symbol/sym-1f97a/)
- [SYM 26D9](https://baroque-curse-text-56.pages.dev/symbol/sym-26d9/)
- [OPEN CENTRE STAR](https://minimal-star-symbols-43.pages.dev/symbol/open-centre-star/)
- [SYM 2657](https://coquette-aesthetic-symbols-51.pages.dev/symbol/sym-2657/)
- [SYM 1D458](https://pastel-moe-kaomoji-91.pages.dev/symbol/sym-1d458/)
- [SYM 1D49B](https://clean-line-emojis-77.pages.dev/symbol/sym-1d49b/)
- [SYM 1D451](https://neon-futuristic-symbols-58.pages.dev/symbol/sym-1d451/)
- [GEMINI ZODIAC TWINS](https://chibi-kaomoji-vault-58.pages.dev/symbol/gemini-zodiac-twins/)
- [SYM 1D44D](https://anime-sparkle-text-24.pages.dev/symbol/sym-1d44d/)
- [SYM 26E8](https://pure-line-unicode-95.pages.dev/symbol/sym-26e8/)
- [SYM 1D4A2](https://synth-crosshair-text-47.pages.dev/symbol/sym-1d4a2/)
- [SYM 1D43B](https://soft-pink-fonts-41.pages.dev/symbol/sym-1d43b/)
- [SYM 1D406](https://soft-pink-fonts-41.pages.dev/symbol/sym-1d406/)
- [SWIMMING FISH LEFT](https://minimal-star-symbols-26.pages.dev/symbol/swimming-fish-left/)
- [BRACKETS](https://clean-line-emojis-77.pages.dev/pt/brackets/)
- [SYM 1D453](https://chibi-kaomoji-vault-58.pages.dev/symbol/sym-1d453/)
- [SYM 1D410](https://anime-sparkle-text-81.pages.dev/symbol/sym-1d410/)
- [SYM 2682](https://synth-crosshair-text-47.pages.dev/symbol/sym-2682/)
- [SYM 1F61E](https://gothic-bio-fonts-90.pages.dev/symbol/sym-1f61e/)
- [SYM 26DF](https://minimal-star-symbols-95.pages.dev/symbol/sym-26df/)
- [SYM 1F49E](https://angelic-bio-symbols-59.pages.dev/symbol/sym-1f49e/)
- [NATURE FLOWERS](https://chibi-emoticon-vault-78.pages.dev/nature-flowers/)
- [SYM 1D414](https://soft-pink-fonts-41.pages.dev/symbol/sym-1d414/)
- [SYM 1D41D](https://soft-pink-fonts-41.pages.dev/symbol/sym-1d41d/)
- [SYM 262B](https://classic-poetry-fonts-16.pages.dev/symbol/sym-262b/)
- [SYM 26E9](https://neon-glitch-symbols-29.pages.dev/symbol/sym-26e9/)
- [SYM 2642](https://coquette-aesthetic-symbols-51.pages.dev/symbol/sym-2642/)
