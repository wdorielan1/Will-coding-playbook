# Inbox

New saves (Instagram screenshots, GitHub links) that haven't been sorted yet. Nothing here is a rule, and none of it applies when building a screen.

## How to sort an entry

1. Turn it into one short, clear rule in plain text. Keep it only if it would change how a screen gets built.
2. Drop it if it is obvious, generic, or already covered by an existing rule.
3. If it contradicts an existing rule, do not file it. List both rules under **Conflicts** and wait for Will to pick one.
4. File it in the matching `references/` file. Use `SKILL.md` core rules only if the rule holds on every screen.
5. Remove the entry from **Unsorted** once it is filed, dropped, or moved to Conflicts.

## Unsorted

### thinking-orbs: https://github.com/Jakubantalik/thinking-orbs (MIT)

Animated "AI is working" loading indicators for chat and agent screens. Needs a topic: none of the six covers loading or AI-status screens. Suggested: a new `references/ai-and-loading-states.md`.

Rules:
- Match the loading animation to what is happening (searching, working, listening…) instead of one generic spinner for every wait. Name the specific action in its accessible label, e.g. "Analysing repository…".
- Build two sizes on purpose: about 20px next to text and about 64px as a chat avatar. Tune each one; don't scale one down.
- Keep the indicator one color and follow the theme: light on dark backgrounds, dark on light.
- With reduced motion on, show one still frame instead of the animation or nothing.

Tool: `thinking-orbs` (React 18+), `<ThinkingOrb state="searching" size={64} />`

Dropped as library internals the package already handles: pausing when offscreen, canvas-only rendering, theme detection, speed and pause props.

Conflicts: none. Duplicates: none.

## Conflicts — pick one

_None._

Format for each conflict:

```
- Topic: <what the rules disagree about>
  - A (filed in references/<file>.md): <rule>
  - B (new, from <source>): <rule>
  - Pick: <Will fills in A, B, or a rewrite>
```
