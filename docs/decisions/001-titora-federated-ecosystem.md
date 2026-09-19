# ADR-001: TITORA Is a Federated Personal Project Ecosystem

- **Status:** Accepted
- **Date:** 2026-09-19
- **Scope:** TITORA repository and public ecosystem map

## Context

TITORA contains a growing set of independent projects spanning product experiments, knowledge systems, growth systems, infrastructure research, and resilience-oriented systems.

Several projects have conceptual relationships. For example, the 11 infrastructure/research systems share a reasoning chain from historical reconstruction through change detection, investigation, incident reconstruction, recovery, orchestration, and human intervention.

Conceptual relationships can create pressure to centralize code, infrastructure, data, or deployment. That would make the index harder to maintain and would blur project ownership.

## Decision

TITORA is treated as a **federated personal project ecosystem**.

TITORA provides:

- project discovery
- public architecture context
- cross-project terminology
- documented relationships
- architecture decisions
- ecosystem-level governance

Individual projects retain ownership of:

- implementation
- runtime state
- data
- deployment
- project-specific security
- project-specific release status
- project-specific operational decisions

A relationship between projects is not an implementation dependency unless an explicit contract is introduced.

## Contract requirement

Any future cross-project integration should define, at minimum:

- purpose
- owning project
- inputs and outputs
- schema/versioning
- failure behavior
- retry/idempotency expectations
- trust boundary
- observability
- ownership of resulting state

## Consequences

### Positive

- Projects remain independently understandable.
- Experimental systems can evolve without destabilizing unrelated projects.
- Public documentation can describe relationships without pretending they are runtime dependencies.
- Integration decisions become explicit and reviewable.

### Trade-offs

- Some information may be duplicated across repositories.
- Cross-project discovery requires documentation discipline.
- Shared functionality may occasionally be reimplemented until a stable contract justifies extraction.

## Rejected alternative

**Build TITORA as a monolithic platform.**

This was rejected because the current projects have different domains, maturity levels, and responsibilities. Centralizing them would introduce coupling before a concrete need exists.
