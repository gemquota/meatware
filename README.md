# Organoids

> Project documentation index. Status snapshot: 14 November 2026.

Organoids is an emergent artificial-life simulation and architectural successor to VEPA. Its central design objective is to build complex, interacting artificial life from a compact, general-purpose substrate rather than implement every organism and behaviour as a bespoke system.

The project is being developed from a deliberately golfed minimal core. The core is a foundation to grow from, not a target to which the entire application must be compressed.

## Documentation

- [Project overview](docs/organoids/PROJECT.md): purpose, scope, lineage and governing principles.
- [Feature catalogue](docs/organoids/FEATURES.md): feature inventory, grouped by capability and implementation confidence.
- [Project status](docs/organoids/STATUS.md): measured artifacts, completed work, current state, risks and verification gaps.
- [Architecture](docs/organoids/ARCHITECTURE.md): substrate, entities, state, rules, modules and emergence.
- [Consolidated specification](docs/organoids/SPECIFICATION.md): the coherent architecture derived from the nine decision areas and confirmed rule model.
- [Source audit](docs/organoids/SOURCE_AUDIT.md): verified state of the live Organoids repository and discrepancies against historical measurements.
- [Execution semantics](docs/organoids/EXECUTION_SEMANTICS.md): rule snapshots, phases, atomic effects, conflict handling, events and reproducibility.
- [Decisions and constraints](docs/organoids/DECISIONS.md): authoritative project boundaries and design decisions.
- [Roadmap](docs/organoids/ROADMAP.md): ordered work programme and acceptance criteria.

## Current source-of-truth note

Project discussion identifies `accretion.html` as the central Organoids artifact and the place from which the system is being built up through progressive golfing and generalisation. Historical discussion also refers to `emergence.js` as an earlier implementation attempt. These are project-history facts, not a claim that this repository currently contains or verifies those files.

## Status at a glance

- **Architecture:** unified emergent-life substrate is the intended direction.
- **Core philosophy:** minimal, golfed, general-purpose primitives; complexity should emerge through composition.
- **Consolidation:** multiple consolidation and abstraction passes have been requested and investigated.
- **Verification:** current source, tests, CI and runtime were not independently available for this documentation import.
- **Next priority:** reconcile the documented architecture and feature inventory against the actual `accretion.html` implementation, then continue measured consolidation.

All implementation-status claims are deliberately qualified where direct source verification is unavailable.
