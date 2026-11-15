---
name: will-ui-playbook
description: Will's personal UI and UX rules, applied to every app Will builds. Use whenever designing, building, reviewing or restyling any user-facing screen, page or component — onboarding, signup and forms, dashboards, mobile layouts, typography and color, landing pages, AI and agent loading states. Read the core rules below first, then the one or two reference files that match the screen.
---

# Will's UI/UX Playbook

## When to use

Any time a user-facing screen, page or component is being designed, built, reviewed or restyled in any of Will's apps. Skip for backend-only work.

## Core rules

These apply to every screen, whatever the topic.

_None chosen yet. A rule belongs here only if it changes how every screen is built. Anything specific to one kind of screen goes in its reference file instead._

## Which reference to read

Read the file that matches the screen's main job. Read a second one when the screen spans topics (a mobile signup form: `forms-and-signup.md` + `mobile-layout.md`).

| Building… | Read |
|---|---|
| What happens after the account exists: welcome, setup steps, permission prompts, first empty states, tours | `references/onboarding.md` |
| Account creation, login, checkout, settings, or any screen whose job is collecting input | `references/forms-and-signup.md` |
| Dashboards, data tables, charts, KPIs, filters, admin or analytics views | `references/dashboards.md` |
| Phone-sized layout: navigation, thumb reach, touch targets, spacing, responsive behavior | `references/mobile-layout.md` |
| Type scale, fonts, color palette, contrast, dark mode | `references/typography-color.md` |
| Marketing pages: hero, value proposition, social proof, pricing, calls to action | `references/landing-pages.md` |
| AI or agent screens: loading indicators, "thinking" and status states, chat waiting states | `references/ai-and-loading-states.md` |

## Do not read while building

`inbox.md` holds saves that haven't been sorted. Nothing in it is a rule yet, so never apply it to a screen. Open it only when asked to sort new saves. The sorting steps are at the top of that file.
