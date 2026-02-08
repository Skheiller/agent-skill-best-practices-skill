# Frontmatter Guidelines

## Required baseline

- `name`: lowercase hyphen-case, <=64 chars.
- `description`: what + when to use, with explicit activation context.

## Description quality checklist

- State domain and concrete task class.
- State activation contexts (file types, intents, scenarios).
- State exclusions if confusion is likely.
- Keep wording operational and unambiguous.

## Platform-sensitive notes

Some ecosystems support additional fields (for example `allowed-tools`, `model`, `disable-model-invocation`).
Use only fields supported by the target platform and document assumptions.

## Strong pattern

"Standardize X for Y workflow. Use when A/B/C. Exclude D."

## Weak pattern

"General helper for many things".
