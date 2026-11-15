# Inbox: the one list

For now every rule goes in this one list, in the order saved, with no topic sorting. The topic files in `references/` stay empty until this list is sorted into them later.

## How a save gets added

1. Turn it into one short, clear rule in plain text. Keep it only if it would change how a screen gets built.
2. Drop it if it is obvious, generic, or already covered by a rule in the list.
3. If it contradicts a rule in the list, do not add it. List both under **Conflicts** and wait for Will to pick one.
4. Add it to **Rules** with its source name in parentheses.

## Rules

- Match the loading animation to what is happening (searching, working, listening…) instead of one generic spinner for every wait. Name the specific action in its accessible label, e.g. "Analysing repository…". (thinking-orbs)
- Build two sizes on purpose: about 20px next to text and about 64px as a chat avatar. Tune each one; don't scale one down. (thinking-orbs)
- Keep the indicator one color and follow the theme: light on dark backgrounds, dark on light. (thinking-orbs)
- With reduced motion on, show one still frame instead of the animation or nothing. (thinking-orbs)
- For AI and agent loading indicators, the `thinking-orbs` package (React 18+) does all of the above: `<ThinkingOrb state="searching" size={64} />`. Source: https://github.com/Jakubantalik/thinking-orbs (MIT). (thinking-orbs)

## Conflicts — pick one

_None._

Format for each conflict:

```
- Topic: <what the rules disagree about>
  - A (in the list): <rule>
  - B (new, from <source>): <rule>
  - Pick: <Will fills in A, B, or a rewrite>
```
