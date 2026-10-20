---
name: awesome-design-md
description: Build UI in the visual style of a well-known site (Stripe, Linear, Apple, Airbnb, Notion, Vercel, Tesla and ~80 more) using ready-made DESIGN.md files of colors, type, spacing and components. Use when the user asks for a page, app screen or component that looks like, feels like or is inspired by a named brand or site, or wants a ready design system to start from.
---

# Awesome DESIGN.md

`design-md/<brand>/DESIGN.md` holds a plain-text design system for each brand: YAML front matter of tokens
(colors, typography, spacing, radii, shadows, components) and prose on how the style is used.

## Workflow

1. List `design-md/` and pick the folder that matches the brand the user named. If none matches, pick the
   closest in feel and say which one you used.
2. Read that `DESIGN.md` in full before writing any UI.
3. Copy it to the project root as `DESIGN.md` (unless the user says not to) so later work stays consistent.
4. Build with its tokens: map colors, type scale, spacing and radii to CSS variables or the project's theme,
   and follow its component and layout rules rather than generic defaults.
5. These are *inspired* interpretations. Never copy logos, trademarks or proprietary fonts; use the
   fallback font stacks it lists.

Source: https://github.com/VoltAgent/awesome-design-md (MIT, see LICENSE).
