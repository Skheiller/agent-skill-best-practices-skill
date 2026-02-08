# Security and Governance for Skills

## Threat model

Skills can execute commands and read/write files. Treat them as code with supply-chain risk.

## Minimum controls

- Pin dependency versions for scripted installs.
- Avoid broad `npx`/remote execution without trust boundary.
- Restrict tool/command scope where platform supports it.
- Document sensitive-path behavior explicitly.

## Governance metadata recommendations

Where supported by platform policy, maintain:

- skill version
- owner/team
- review date
- risk level
- approved execution patterns

## Review cadence

- Re-review skills after major runtime/toolchain updates.
- Re-review immediately after incidents or suspicious behavior.
