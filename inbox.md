# Inbox

New saves (Instagram screenshots, GitHub links) that haven't been sorted yet. Nothing here is a rule, and none of it applies when building a screen.

## How to sort an entry

1. Turn it into one short, clear rule in plain text. Keep it only if it would change how a screen gets built.
2. Drop it if it is obvious, generic, or already covered by an existing rule.
3. If it contradicts an existing rule, do not file it. List both rules under **Conflicts** and wait for Will to pick one.
4. File it in the matching `references/` file. Use `SKILL.md` core rules only if the rule holds on every screen. If no topic fits, create a new file in `references/` named for the topic and add its row to the table in `SKILL.md`. Don't wait to ask.
5. Remove the entry from **Unsorted** once it is filed, dropped, or moved to Conflicts.

## Bulk saves: doomer-agent

For a pile of saved reels, use the `doomer-agent` skill (https://github.com/jnh12/doomer-agent, MIT). It studies videos and writes up what they teach. It does not touch GitHub.

- Run it in the Claude app, with Claude in Chrome signed into Instagram. This cloud session can't reach a signed-in Instagram.
- Do 5–15 reels on one topic at a time. Video analysis uses a lot of the usage allowance.
- Tell it the job is "UI/UX rules for will-ui-playbook" and to give rules, not new skills.
- Paste what it produces here, then sort it with the steps above.

## Unsorted

_Empty._

## Conflicts — pick one

_None._

Format for each conflict:

```
- Topic: <what the rules disagree about>
  - A (filed in references/<file>.md): <rule>
  - B (new, from <source>): <rule>
  - Pick: <Will fills in A, B, or a rewrite>
```
