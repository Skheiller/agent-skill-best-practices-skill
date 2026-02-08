---
name: agent-skill-best-practices
description: Research-backed quality framework for creating and upgrading SKILL.md-based agent capabilities. Use when designing new skills, auditing existing skills, reducing context bloat, improving trigger precision, adding safe tool boundaries, or migrating skills across Codex, Claude Code, and Copilot-style environments.
---

# Agent Skill Best Practices

## Overview

Use this skill to engineer better skills with measurable quality gates: precise activation, efficient context usage, executable workflows, and safe operational boundaries.

This skill is intended for skill authors and reviewers.

## Research-Backed Standards

Apply these baseline standards before any custom style decisions:

- Keep `SKILL.md` lean and move deep detail to `references/`.
- Prefer progressive disclosure (metadata -> body -> resources on demand).
- Keep reference depth shallow (link directly from `SKILL.md`, avoid deep chains).
- Use imperative instructions with explicit completion conditions.
- Treat scripts and command guidance as production code with risk controls.

Load citations in `references/evidence-2026.md` when needed.

## Workflow

1. Determine mode.
- `create`: build a new skill.
- `upgrade`: improve an existing skill.
- `audit`: score and report findings.
- `migrate`: adapt to another agent platform.

2. Define target contract.
- Required behaviors.
- Trigger phrases/contexts.
- Supported platforms.
- Risk tolerance and execution boundaries.

3. Run structured audit.
- Score with `references/audit-rubric.md`.
- Record severity-ranked findings using `references/review-template.md`.

4. Implement fixes in strict order.
- Frontmatter precision.
- Body structure and progressive disclosure.
- Deterministic workflow and output contract.
- Security/governance boundaries.
- Cross-platform portability.

5. Validate and finalize.
- Run `quick_validate.py` where available.
- Return change summary, remaining risks, and next iteration items.

## Non-Negotiable Rules

- No TODO placeholders in production skill files.
- No broad/vague description that can trigger everywhere.
- No monolithic SKILL body when detail can live in references.
- No unbounded command execution guidance for risky operations.
- No hidden platform assumptions (paths, tool availability, shell behavior).

## Required Outputs Per Engagement

- Updated skill files.
- Findings list ordered by severity.
- Validation result.
- Residual risk statement.

## References

Load only relevant references for the current job.

- Evidence and source links: `references/evidence-2026.md`
- Scoring framework: `references/audit-rubric.md`
- Frontmatter design: `references/frontmatter-guidelines.md`
- Body design and progressive disclosure: `references/body-design-patterns.md`
- Security and governance: `references/security-governance.md`
- Portability/migration: `references/interoperability-migration.md`
- Anti-patterns: `references/anti-patterns.md`
- Review output format: `references/review-template.md`
