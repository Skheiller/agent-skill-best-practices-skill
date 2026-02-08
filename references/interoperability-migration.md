# Interoperability and Migration

## Portability principles

- Keep core logic in markdown + simple scripts.
- Isolate platform-specific options in clearly marked sections.
- Document paths, shell assumptions, and required tools.

## Common skill locations

- Claude project skills: `.claude/skills/`
- Claude user skills: `~/.claude/skills/`
- Codex skills: `$CODEX_HOME/skills` (environment-dependent)
- Copilot customization is repository/user scoped via instruction files.

## Migration checklist

1. Normalize naming and description precision.
2. Remove unsupported metadata fields for target platform.
3. Re-map path assumptions and tool policies.
4. Re-test activation behavior with representative prompts.
5. Re-run safety and validation checks.

## Cross-platform caution

Discovery semantics and execution permissions differ by platform.
Always declare assumptions explicitly inside the skill.
