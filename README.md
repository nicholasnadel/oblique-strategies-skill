# Oblique Strategies

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill that brings Brian Eno and Peter Schmidt's [Oblique Strategies](https://en.wikipedia.org/wiki/Oblique_Strategies) into your coding sessions.

> *Over One Hundred Worthwhile Dilemmas*

## What it does

Draws a single card from the Oblique Strategies deck when you're stuck. One card. No re-draws. Sit with it.

The skill detects when you're going in circles and offers a card — or you can invoke it directly with `/oblique`. It presents the card in its original voice, then offers a brief interpretation in the context of whatever you're working on.

## What it won't do

- **Draw when things are going fine.** This is medicine, not vitamins.
- **Let you reject a card and re-draw.** The constraint is the creative act.
- **Flatten the cards into engineering platitudes.** "Use fewer notes" stays "Use fewer notes" — it doesn't become "Reduce API surface area."

## Install

```bash
claude skill add --from nicholasnadel/oblique-strategies-skill
```

Or clone directly into your skills directory:

```bash
git clone git@github.com:nicholasnadel/oblique-strategies-skill.git ~/.claude/skills/oblique-strategies
```

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
