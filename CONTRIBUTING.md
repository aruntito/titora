# Contributing to TITORA

TITORA is an ecosystem-level architecture and documentation repository. Contributions should improve clarity, correctness, maintainability, or the quality of the systems described here.

## What belongs here

Good contributions include:

- architecture documentation
- system boundaries and contracts
- diagrams
- architecture decision records
- cross-project conventions
- operational and security documentation
- documentation fixes

Implementation code should normally live in the repository that owns the system.

## Before changing architecture

A proposed architecture change should answer:

1. What problem does this solve?
2. Which system owns the responsibility?
3. What new coupling does it introduce?
4. What happens when the dependency fails?
5. How is the behavior observed and recovered?
6. Can the component be replaced without redesigning the ecosystem?

Avoid adding abstractions simply because multiple systems look similar. Shared infrastructure is valuable only when the shared contract is stable.

## Contribution workflow

1. Create a focused branch.
2. Make the smallest coherent change.
3. Update related documentation and diagrams.
4. Use Conventional Commits such as `docs:`, `feat:`, `fix:`, or `chore:`.
5. Open a pull request explaining the architectural or operational impact.

## Documentation standards

- Prefer concrete language over marketing language.
- Separate current capabilities from future direction.
- Do not describe planned functionality as production-ready.
- Keep diagrams synchronized with the written architecture.
- Link to the owning repository when implementation details live elsewhere.

## Pull request checklist

- [ ] The change has a clear purpose.
- [ ] System ownership is explicit.
- [ ] Documentation matches the current state.
- [ ] Diagrams remain accurate.
- [ ] No secrets or private infrastructure details are included.
- [ ] The change does not introduce unnecessary cross-system coupling.
