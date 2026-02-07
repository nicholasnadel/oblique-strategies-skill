# Oblique Strategies

A system prompt for any LLM that brings Brian Eno and Peter Schmidt's [Oblique Strategies](https://en.wikipedia.org/wiki/Oblique_Strategies) into your creative and coding sessions.

> *Over One Hundred Worthwhile Dilemmas*

## What it does

Draws a single card from the Oblique Strategies deck when you're stuck. One card. No re-draws. Sit with it.

The LLM detects when you're going in circles and offers a card — or you can ask for one directly. It presents the card in its original voice, then offers a brief interpretation in the context of whatever you're working on.

## What it won't do

- **Draw when things are going fine.** This is medicine, not vitamins.
- **Let you reject a card and re-draw.** The constraint is the creative act.
- **Flatten the cards into engineering platitudes.** "Use fewer notes" stays "Use fewer notes" — it doesn't become "Reduce API surface area."

## Install

The core of this repo is `SKILL.md` — a plain markdown file containing the full deck and behavioral instructions. Any LLM that can read a system prompt can use it. Pick the method that fits your tool:

### Claude Code

```bash
claude skill add --from nicholasnadel/oblique-strategies-skill
```

Or clone directly:

```bash
git clone https://github.com/nicholasnadel/oblique-strategies-skill.git ~/.claude/skills/oblique-strategies
```

### Cursor

Copy `SKILL.md` into your project's rules directory:

```bash
cp SKILL.md .cursor/rules/oblique-strategies.md
```

Or add it as a global rule at `~/.cursor/rules/oblique-strategies.md`.

### Windsurf

Copy `SKILL.md` into your Windsurf rules:

```bash
cp SKILL.md .windsurf/rules/oblique-strategies.md
```

### GitHub Copilot

Copy `SKILL.md` into your Copilot instructions:

```bash
cp SKILL.md .github/copilot-instructions/oblique-strategies.md
```

### ChatGPT / Custom GPTs

1. Open **Settings > Personalization > Custom Instructions** (or create a Custom GPT)
2. Paste the contents of `SKILL.md` into the system instructions

### Any other LLM

Paste the contents of `SKILL.md` into whatever system prompt, custom instructions, or rules file your tool supports. It's just markdown — no proprietary format, no dependencies.

## Example

You've been refactoring the same function for 20 minutes, trying different approaches that all feel wrong:

> **"Discover the recipes you are using and abandon them"**
>
> — Oblique Strategies, Eno/Schmidt

*You keep reaching for the same pattern — extract, rename, inline. What if the function shouldn't exist at all? What if the caller should own this logic directly?*

## About Oblique Strategies

Originally published in 1975 as a deck of printed cards. Each card contains a brief instruction or provocation designed to break creative deadlocks through lateral thinking. Created by musician Brian Eno and artist Peter Schmidt.

The deck contains 114 cards, including one blank white card.

## License

The Oblique Strategies themselves are the creative work of Brian Eno and Peter Schmidt. This skill is an unofficial fan implementation for personal use in AI-assisted creative work.
