# Evidence Base (2025-2026)

This reference anchors recommendations in primary sources.

## 1) Agent Skills specification

Source: agentskills.io
- Standardized `SKILL.md` with YAML frontmatter and markdown body.
- Cross-framework positioning and reusable capability packaging.

Link: https://agentskills.io

## 2) Claude skills best practices and structure

Sources: docs.claude.com + support.claude.com
- Progressive disclosure model (metadata first, full body on match).
- Keep `SKILL.md` lean; split large content into `references/`.
- Guidance to keep core SKILL body under roughly 500 lines.
- Prefer one-level-deep references from SKILL body.
- Common storage paths:
  - Project skills: `.claude/skills/`
  - User skills: `~/.claude/skills/`
- Optional frontmatter controls in Claude ecosystem include fields such as `allowed-tools`, `model`, and `disable-model-invocation`.

Links:
- https://docs.claude.com/en/docs/claude-code/skills
- https://support.claude.com/en/articles/11752874-creating-custom-skills-for-claude-code

## 3) Official Anthropic skills repository patterns

Source: github.com/anthropics/skills
- Template emphasizes concise metadata, imperative body instructions, and optional resource folders (`scripts`, `references`, `assets`).
- Includes a `skill-creator` meta-skill for structured authoring and validation workflow.

Link: https://github.com/anthropics/skills

## 4) GitHub Copilot custom instruction framework

Source: docs.github.com (Customizing Copilot)
- Establishes repository/user-scoped instruction organization for repeatable behavior.
- Reinforces directory-based, versionable instruction artifacts.

Link: https://docs.github.com/en/copilot/concepts/about-customizing-github-copilot-chat-responses

## 5) Design rationale for composability

Source: Anthropic engineering blog on context engineering (July 2025)
- Argues for composable prompts and small task-focused instruction units.
- Supports modular skill design to preserve context and reasoning quality.

Link: https://www.anthropic.com/engineering/context-engineering-for-agents

## Usage rule

When proposing a best practice, tie it to one or more sources above.
