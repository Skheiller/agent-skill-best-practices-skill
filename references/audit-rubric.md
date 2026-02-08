# Skill Audit Rubric

Score each category 0-5. Target >= 4 in every category.

## 1) Trigger Precision

- `0`: vague description, broad activation surface.
- `3`: mostly clear but overlaps many unrelated tasks.
- `5`: explicit scope, exclusions, and concrete activation contexts.

## 2) Context Efficiency

- `0`: large monolithic SKILL body, duplicated content.
- `3`: partial separation into references.
- `5`: progressive disclosure is clear; heavy detail lives in `references/`.

## 3) Workflow Correctness

- `0`: unordered tips, no execution path.
- `3`: sequence exists but branching unclear.
- `5`: deterministic steps, clear decision points, explicit outputs.

## 4) Safety & Governance

- `0`: unrestricted command guidance, unpinned dependencies.
- `3`: basic cautions, limited enforceable controls.
- `5`: explicit boundaries, tool allowlists, ownership/versioning guidance.

## 5) Portability

- `0`: platform-specific assumptions are hidden.
- `3`: some assumptions documented.
- `5`: required environment assumptions, path rules, and migration notes are explicit.

## 6) Maintainability

- `0`: hard to update; no structure.
- `3`: partial organization.
- `5`: modular references, clear naming, easy extension points.

## Exit Criteria

- No category below `4`.
- No unresolved high-severity safety finding.
