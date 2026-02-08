# Agent Skill Best Practices

A research-backed meta-skill for creating, auditing, upgrading, and migrating `SKILL.md`-based capabilities.

## What It Does

- Audits skill quality using a scoring rubric.
- Improves trigger precision and progressive disclosure.
- Tightens safety/governance boundaries for executable guidance.
- Helps port skills across Codex/Claude/Copilot-style environments.

## Included Research Basis

Primary-source evidence is documented in:

- `references/evidence-2026.md`

That file captures the standards used to shape this skill, including official docs/specs and ecosystem guidance.

## Structure

- `SKILL.md`: main playbook and quality gates
- `agents/openai.yaml`: UI metadata
- `references/`: rubric, anti-patterns, frontmatter/body guidance, security, migration, template

## Quick Use Prompt

`Use $agent-skill-best-practices to audit and improve this skill to production quality.`

## Typical Engagement Outputs

- Severity-ranked findings (`high/medium/low`)
- File-level updates
- Validation result
- Residual-risk statement

## Validation

```bash
python3 /Users/lmostafa/.codex/skills/.system/skill-creator/scripts/quick_validate.py .
```

## License

MIT
