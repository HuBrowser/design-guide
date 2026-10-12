# Design Guide for AI Coding Agents

Lightweight design guidance for AI coding agents building and improving Web and Mobile App UI. Make deliberate choices about layout, typography, color, and interaction based on the product and its users.

The goal is better visual judgment: clear hierarchy, coherent expression, and usable interfaces that do not look interchangeable. A gradient, rounded card, or neutral font can be the right choice. The problem is applying the same treatment regardless of the task.

## What you get

- **Context-aware design:** start with the user outcome and respect established brands and design systems.
- **Practical judgment:** diagnose weak composition and unnecessary UI before adding decoration.
- **Appropriate effort:** handle small improvements directly; think more deeply when the product needs a redesign.
- **Portable guidance:** plain Markdown for Codex, Claude Code, GitHub Copilot, and other agents. No extra programs, packages, framework, or component library required.

[DESIGN.md](DESIGN.md) is the sole source of general design principles. [SKILL.md](SKILL.md) is a small Agent Skills entry point that loads it. Use the guide for new interfaces, focused UI improvements, visual critique, or an explicitly requested redesign.

## Copy-paste prompt

Once this repository is published, paste this into an agent with URL-reading access:

```text
Read https://raw.githubusercontent.com/HuBrowser/design-guide/main/DESIGN.md
and apply it to this task: [describe the product, UI surface, and desired outcome].

Use the project's existing design system and behavior as the starting point.
Treat the task as a refinement unless I explicitly request a redesign.
Follow explicit product requirements over generic preferences. Keep the work
proportional to the change. Review the rendered result when available and
authorized, and state any verification limits.

If you cannot retrieve the guide, tell me so I can provide the local file.
```

You can also attach `DESIGN.md` directly or ask the agent to read a local copy. A URL alone does not guarantee that an agent can fetch its contents.

## Optional integration

Copy `SKILL.md`, `DESIGN.md`, and `LICENSE` together into a folder named `design-guide` in one of these locations:

| Agent | Project folder | Personal folder | Explicit use |
| --- | --- | --- | --- |
| Codex | `.agents/skills/design-guide/` | `~/.agents/skills/design-guide/` | Ask to use `$design-guide` |
| Claude Code | `.claude/skills/design-guide/` | `~/.claude/skills/design-guide/` | Use `/design-guide` with your task |
| GitHub Copilot in VS Code | `.github/skills/design-guide/` | `~/.copilot/skills/design-guide/` | Ask to use the `design-guide` skill |

Choose one scope per agent to avoid duplicate discovery. Supported agents can also select the skill when its description matches the task. Discovery varies by host and version; see the official [Codex](https://developers.openai.com/codex/skills/), [Claude Code](https://code.claude.com/docs/en/skills), and [VS Code Copilot](https://code.visualstudio.com/docs/copilot/customization/agent-skills) documentation.

For hosts without skills support, keep a local copy and add a short instruction to the project's `AGENTS.md`, `CLAUDE.md`, or `.github/copilot-instructions.md`:

```text
For UI design and visual improvements, read the Design Guide at
[relative path to the local guide's DESIGN.md]. Apply its general principles
within this project's requirements and established design system.
```

Keep the guide separate from the product's own `DESIGN.md`. This repository explains how to make decisions; the product file records its actual visual language, tokens, and constraints. The guide does not grant permission to use browsers, desktop apps, paid services, or external publishing tools.

## References and license

Research references include [Anthropic frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design), [Impeccable](https://github.com/pbakaus/impeccable), [UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill), [Taste](https://github.com/tyfarrago-hub/taste), and [ckw-design](https://github.com/connerkward/ckw-design-skill). They offer useful perspectives on intention, critique, and craft; their style prescriptions and tooling are not requirements here. This repository ships independently written guidance, without vendored third-party text, code, or assets. Referenced projects retain their own licenses.

[MIT License](LICENSE). You can use, adapt, and redistribute the guide, including for commercial work, with the license notice retained.
