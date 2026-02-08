# Instruction Body Design Patterns

## Canonical structure

1. Overview (purpose and boundaries)
2. Ordered workflow (execution path)
3. Non-negotiable rules
4. Required outputs
5. Reference map

## Progressive disclosure checklist

- Keep SKILL core body compact (target: well under 500 lines).
- Move dense examples, schemas, and variants into `references/`.
- Link to references directly from SKILL body.
- Avoid deep reference chains (prefer one-level navigation).

## Workflow authoring rules

- Use imperative verbs.
- One action per bullet.
- Include decision points for branching.
- State completion criteria per step.
- State output contract explicitly.

## Determinism rule

For brittle operations (complex parsing, strict transforms), use scripts instead of free-form reasoning.

## Anti-bloat rule

Do not duplicate content between SKILL body and references.
