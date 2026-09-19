# TITORA Projects

TITORA is the public index for Arun Tito's independent personal technology projects.

This is a portfolio map, not a claim that these systems share one runtime, deployment, codebase, or production state.

## Project families

### Core projects

| Project | Role |
| --- | --- |
| TITORA | Personal technology ecosystem and public project index |
| DOOB | Growth intelligence, orchestration, and execution |
| KARADAVI | Knowledge and semantic infrastructure |
| SMXM | Growth, marketing, media operations, and distribution |
| CAMERA APP | Creator-focused camera and recording workflow |
### Infrastructure & research family

| Project | Mission | Core question |
| --- | --- | --- |
| TIME-MACHINE | Historical state reconstruction | How did we get here? |
| PULSE | Meaningful change detection | What just changed? |
| TRACE | Causal investigation | Why did it change? |
| BLACKBOX | Forensic incident reconstruction | What actually happened? |
| RECOVER | Controlled recovery and restoration | How do we get back to a known-good state? |
| FIRSTLIGHT | First-hour incident orchestration | What should happen first? |
| WAKE | Human escalation and intervention routing | Who needs to act? |
| GRID | Infrastructure dependency graph | What is connected to what? |
| GHOST | Unknown/orphaned infrastructure discovery | What exists that we don't know about? |
| EVAC | Evacuation simulation and resilience research | How does a system respond under pressure? |
| RELIEF-OS | Resource and logistics coordination | How do we allocate help effectively? |

## Conceptual relationship

```text
Historical state
TIME-MACHINE
      ↓
Change
PULSE
      ↓
Investigation
TRACE
      ↓
Incident reconstruction
BLACKBOX
      ↓
Recovery
RECOVER
      ↓
Initial response
FIRSTLIGHT
      ↓
Human intervention
WAKE
```

Contextual systems:

- **GRID** → dependency and topology context
- **GHOST** → unknown/orphan/inventory context
- **EVAC** → simulation and resilience research
- **RELIEF-OS** → resource and logistics context

These relationships describe problem adjacency, not mandatory runtime dependencies.

## Independence rule

A project should not import, deploy, or depend on another TITORA project merely because the concepts are related.

Integration requires a concrete reason and an explicit contract.

## Status language

- **Concept** — defined problem or research direction.
- **Planned** — intentionally selected for future work.
- **Implemented** — functionality exists and has been checked.
- **Verified** — behavior has been explicitly tested or otherwise verified.
- **Production** — deployed and operating in a real environment.

Documentation alone does not move a project into the last three categories.
