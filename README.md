# media

Claude Code skills for design and media work. This branch is separate from the Minecraft server
config on `main` and shares no history with it.

The skills are the five repos from Henry Chua's reel (credited to Nate Herk), "5 free repos that make
Claude a designer". They live in `.claude/skills/`, so Claude Code picks them up when you open this
branch as a project. To use them everywhere, copy the folders into `~/.claude/skills/`.

| Skill | What it does | Upstream (pinned commit) |
|-------|--------------|--------------------------|
| `taste-skill` (`design-taste-frontend`) | Art direction and anti-slop rules for landing pages and app screens | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) @ `63aba5f` |
| `impeccable` | Design, critique, audit and polish frontend UI; `/impeccable audit`, `polish`, etc. | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) @ `e7d0f58` |
| `playwright-cli` | Drive a real browser to screenshot and test pages | [microsoft/playwright-cli](https://github.com/microsoft/playwright-cli) @ `b1a5903` |
| `awesome-design-md` | ~84 DESIGN.md design systems inspired by well-known sites | [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) @ `3b60532` |
| `img2threejs` | Turn a reference image into a procedural Three.js model | [img2threejs/img2threejs](https://github.com/img2threejs/img2threejs) @ `d508b59` |

## Requirements

- `playwright-cli`: `npm install -g @playwright/cli@latest` (Node 18+).
- `img2threejs`: Python 3.10+.
- `awesome-design-md` has no upstream SKILL.md; the one here was written for this branch.

The reel also used Higgsfield (a paid AI image/video tool) to make the 3D scroll frames. It is a web
service, not a skill, so it isn't included.

Each skill folder keeps its upstream LICENSE.
