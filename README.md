# Workflow and design guides for AI agents

Lightweight guidance for coding, research, automation, and UI design. Start from the intended outcome, use the simplest effective workflow, and verify the result with evidence.

Maintained by [HuBrowser](https://github.com/HuBrowser).

## Choose a guide

| Guide | Use it for |
| --- | --- |
| [WORKFLOW.md](WORKFLOW.md) | Goals, acceptance criteria, execution, research, bounded recovery, checkpoints, verification, and handoff. |
| [DESIGN.md](DESIGN.md) | UI composition, typography, color, interaction, accessibility, responsive behavior, and rendered critique. |
| [SKILL.md](SKILL.md) | An optional Agent Skills entry point that selects the relevant guide. |

Read the guide relevant to your task. Use both for UI implementation. Plain Markdown, with no required tools or dependencies.

For a focused visual critique, start with `DESIGN.md`. For execution or workflow review, start with `WORKFLOW.md`. Neither guide replaces project instructions or the product's design system.

## Quick start

Share this prompt with your agent:

```text
Read https://raw.githubusercontent.com/HuBrowser/design-guide/main/WORKFLOW.md
and apply it to this task: [describe the task and intended outcome].

If the task involves UI design or visual improvements, also read
https://raw.githubusercontent.com/HuBrowser/design-guide/main/DESIGN.md
and use the project's existing design system.

Respect project instructions and permissions. Keep effort proportional,
verify the outcome, and state any verification limits.

If you cannot retrieve a guide, say which file is unavailable so I can
provide a local copy. Do not claim to have read an unavailable guide.
```

You can also attach the Markdown files or provide a local path.

## Optional integration

Copy `SKILL.md`, `WORKFLOW.md`, `DESIGN.md`, and `LICENSE` into a `design-guide` folder at one of these locations:

| Agent | Project folder | Personal folder | Explicit use |
| --- | --- | --- | --- |
| Codex | `.agents/skills/design-guide/` | `~/.agents/skills/design-guide/` | Ask to use `$design-guide` |
| Claude Code | `.claude/skills/design-guide/` | `~/.claude/skills/design-guide/` | Use `/design-guide` with your task |
| GitHub Copilot in VS Code | `.github/skills/design-guide/` | `~/.copilot/skills/design-guide/` | Ask to use the `design-guide` skill |

Choose one scope per agent. See the official [Codex](https://developers.openai.com/codex/skills/), [Claude Code](https://code.claude.com/docs/en/skills), and [VS Code Copilot](https://code.visualstudio.com/docs/copilot/customization/agent-skills) documentation for discovery behavior.

Without skills support, reference the relevant guide from your project's agent instructions. Project requirements and host permissions take precedence.

Keep these files together so relative links resolve. Keep this guide separate from the product's own `DESIGN.md`, which records its visual language, components, and constraints. Updating your local copy is a separate, deliberate action; installation does not create an automatic update mechanism.

## References and license

Design references: [Anthropic frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design), [Impeccable](https://github.com/pbakaus/impeccable), [UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill), [Taste](https://github.com/tyfarrago-hub/taste), and [ckw-design](https://github.com/connerkward/ckw-design-skill). Guidance is independently written; referenced projects retain their own licenses.

[MIT License](LICENSE).
