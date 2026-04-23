# frontend-design

Frontend design skill for Claude Code, Codex, and Gemini CLI. Demands a specific reference, a governing move, and an opinion before the code. Refuses to ship generic.

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

Before writing code, the skill demands four specific answers:

1. **What is this surface for?** Not the brand. Not the industry. What does the page *do* for the person reading it?
2. **What specific design does this remind you of?** A real, nameable thing. A site URL, a designer's work, a magazine spread, a record sleeve, a film title sequence. Not a category.
3. **What is the governing move?** The one move someone would remember a month after seeing the design. Not the palette. Not the typeface. The move.
4. **What would a senior designer raise an eyebrow at?** The bold choice. If nothing, the design has no opinion.

Then the HTML+CSS, written to carry those commitments into every visible decision.

## Example

For *"Design a landing page for a Brooklyn punk record label"*, the preamble would look like:

```
1. Serves the label's refusal — streaming-free, vinyl-only, basement
   venue. The page should feel made by the hands that press the records.
2. Feels like Maximum Rocknroll issue 100, January 1992 — the cover
   and the classifieds pages together, not one or the other.
3. A "NOT ON SPOTIFY" rubber stamp, pressed nine times across the page
   at inconsistent angles. The same stamp by the same tired hand. The
   whole page is punctuated by this one gesture.
4. Default browser controls — native select, unstyled button, underlined
   blue links that stay blue. Every other AI would have styled these.
```

Followed by the single-file HTML document implementing each commitment.

## Why this instead of the default skill

Anthropic's default `frontend-design` skill encourages bold direction but treats archetype as a category — "Editorial," "Brutalist," "Maximalist." The result is defensible outputs that could have been made by any competent AI: Fraunces + JetBrains Mono, ivory-and-ink palette, tasteful vermilion accent, paper grain. Different briefs, same production.

This skill refuses category answers. A specific named reference cannot be hedged. A governing move cannot be averaged across options. An eyebrow-raise cannot be tasteful. Together, they force commitment — and the commitment is what makes the output a design rather than a default.

## License

MIT.
