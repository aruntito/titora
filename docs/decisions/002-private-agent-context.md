# ADR-002: Keep Private Agent Context Outside the Public Repository

- **Status:** Accepted
- **Date:** 2026-09-19
- **Scope:** TITORA ecosystem documentation and development workflow

## Context

The projects use local agent-assisted development. Detailed implementation context may include unfinished decisions, local paths, environment details, private infrastructure information, or other material that is not intended for public publication.

The public repositories should remain useful without exposing that private context.

## Decision

Private engineering context may be maintained locally using the following convention where appropriate:

```text
AGENTS.md
.agent/
├── requirements.md
├── data-model.md
├── interfaces.md
├── invariants.md
└── implementation.md
```

The public repository may document the existence and purpose of this layer, but private contents are not treated as public documentation.

## Security boundary

`.gitignore` is not a security control.

Secrets, credentials, tokens, private keys, private customer information, and other sensitive material must never be placed in a repository merely because a path is ignored.

## Consequences

- Public repositories stay focused on intentional public material.
- Local agent workflows can carry richer implementation context.
- Contributors must consciously decide what belongs in public documentation.
- A developer can still accidentally expose private material if they commit it manually, so review remains necessary.
