# Organoids Decisions and Constraints

**Last consolidated:** 14 November 2026

This document records the project boundaries that should govern future implementation and documentation.

## Identity and lineage

1. Organoids is the successor, not sequel, to VEPA.
2. Organoids carries forward VEPA's architectural lineage and generalisation philosophy.
3. GolfCore and the approximately 600–700-byte minimal functional core philosophy belong to Organoids.
4. Organoids is an artificial-life software simulation, not a real-world organoid brain development project.

## Repository and implementation boundaries

5. `accretion.html` is identified in project discussion as the central Organoids artifact.
6. `emergence.js` is a historical/previous implementation attempt whose exact current status must be verified.
7. The intended direction is one coherent architecture, not parallel competing implementations.
8. No Boids code, dependencies, inherited implementation or cross-project changes may enter Organoids.
9. Boids-related concepts may only be independently re-expressed where they fit Organoids' own architecture.
10. Mocean and NEXUS Aquarium remain separate projects.

## Architecture

11. Prefer a unified entity/composition model.
12. Prefer shared physics, fields, constraints and energy engines.
13. Prefer declarative chemical and biological rules.
14. Build higher-order organisation through emergence and composition.
15. Prioritise semantic interoperability, modularisation and reusable primitives.
16. Consolidate before adding redundant specialised mechanisms.
17. Keep the minimal core small while allowing higher-level modules to remain expressive.

## Engineering and reporting

18. Estimates and measurements must be labelled separately.
19. Preserve both total and non-whitespace character counts.
20. Every consolidation pass must include before/after counts.
21. A feature is not complete merely because it has been proposed, discussed or documented.
22. Report tests and runtime verification accurately.
23. Keep unresolved questions visible instead of silently choosing an unsupported implementation.

## Change control

When a proposed change conflicts with these decisions, stop and reconcile the conflict before implementing it. In particular, do not solve a missing Organoids capability by importing another project's implementation.
