# AI and loading states

Read for: screens that show an AI or agent working. Loading indicators, "thinking" and status states, chat waiting states.

## Rules

- Match the loading animation to what is happening (searching, working, listening…) instead of one generic spinner for every wait. Name the specific action in its accessible label, e.g. "Analysing repository…".
- Build two sizes on purpose: about 20px next to text and about 64px as a chat avatar. Tune each one; don't scale one down.
- Keep the indicator one color and follow the theme: light on dark backgrounds, dark on light.
- With reduced motion on, show one still frame instead of the animation or nothing.

## Tool

`thinking-orbs` (React 18+): `<ThinkingOrb state="searching" size={64} />`. Source: https://github.com/Jakubantalik/thinking-orbs (MIT).
