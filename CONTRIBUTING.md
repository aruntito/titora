# Contributing to TITORA

TITORA is Arun Tito's personal technology project ecosystem and public architecture index. This repository maps independent projects; it is not a monorepo or shared runtime.

## What belongs here

Good contributions include:

- ecosystem architecture and project maps
- system boundaries and cross-project contracts
- diagrams and public documentation
- architecture decision records
- contribution, security, and operational guidance
- corrections to project metadata or links

Implementation code should normally live in the repository that owns the system.

## Before changing architecture

A proposed architecture change should answer:

1. What problem does this solve?
2. Which project owns the responsibility?
3. What new coupling does it introduce?
4. What happens when the dependency fails?
5. How is the behavior observed and recovered?
6. Can the component be replaced without redesigning the ecosystem?

Conceptual similarity is not enough reason to create a shared dependency.

## Contribution workflow

1. Create a focused branch.
2. Make the smallest coherent change.
3. Update related documentation and diagrams.
4. Use Conventional Commits such as `docs:`, `feat:`, `fix:`, or `chore:`.
5. Open a pull request that explains the reason and impact.

## Documentation standards

- Prefer concrete language over marketing language.
- Separate current state from future direction.
- Never describe planned or documented behavior as implemented or production-ready without evidence.
- Keep diagrams synchronized with the written architecture.
- Link to the owning repository when implementation details live elsewhere.
- Preserve distinctions between observation, evidence, interpretation, hypothesis, decision, action, and outcome where relevant.

## Public/private boundary

Do not commit secrets, credentials, private infrastructure details, local agent context, or other information that is not intentionally public.

The repository's `.gitignore` is convenience, not a security boundary.

## Pull request checklist

- [ ] The change has a clear purpose.
- [ ] System/project ownership is explicit.
- [ ] Documentation matches the verified public state.
- [ ] Diagrams remain accurate.
- [ ] No secrets or private infrastructure details are included.
- [ ] No unsupported implementation or production claims were added.
- [ ] The change does not introduce unnecessary cross-project coupling.
