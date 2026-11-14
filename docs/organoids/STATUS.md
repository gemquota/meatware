# Organoids Project Status

**Status snapshot:** 14 November 2026  
**Source confidence:** reconstructed from project conversation and reported measurements; current repository/source was not independently inspected for this documentation import.

## 1. Executive status

Organoids is in an architectural consolidation and foundational implementation phase. The project direction is clear: build a compact, golfed, general-purpose substrate and grow the artificial-life system through reusable primitives and composition.

Recent work has focused on analysing implementation size, reconciling the minimal-core philosophy with the actual implementation, and repeatedly investigating consolidation, semantic interoperability, primitive generalisation and universal abstraction.

The largest outstanding risk is status ambiguity: design scope, prior implementation attempts and verified working features have not yet been reconciled into one source-backed inventory.

## 2. Historical source measurements

The following measurements were reported in project discussion on 13 November 2026:

| Artifact | Characters | Non-whitespace |
|---|---:|---:|
| `emergence.js` | 10,531 | 10,126 |
| `accretion.html` | 3,179 | 3,087 |
| Tests | 3,997 | 3,786 |
| Documentation | 2,730 | 2,383 |

These are reported measurements, not estimates. They should be re-run against the current files before being treated as the present baseline.

A separate comparison exposed a major estimate/measurement discrepancy:

| Measure | Estimate | Actual |
|---|---:|---:|
| Shared substrate | 710 | 12,350 |

The actual was approximately 17.4 times the estimate. The discrepancy demonstrates why architectural estimates must not be presented as measured source size.

The 12,350-character shared-substrate measurement is a separate reported measurement. Do not assume it is the sum of the four artifact rows above without confirming the measurement scope and counting method.

## 3. Artifact lineage

### `accretion.html`

Project discussion identifies this as the central and authoritative Organoids artifact. The stated approach is to build the system up from a golfed foundation in this file.

### `emergence.js`

This was discussed as a previous implementation attempt. It has a reported size of 10,531 characters (10,126 non-whitespace). Its exact relationship to the current `accretion.html` implementation, including whether it is superseded, partially reusable as reference, or still active, requires source-level reconciliation.

Do not silently treat both as current parallel implementations. The intended architecture is one coherent system.

### Tests and documentation

Historical measurements exist, but current paths, test coverage, and whether the documentation reflects the latest architecture remain unverified.

## 4. Work reported or requested

- Established Organoids as a VEPA architectural successor rather than a sequel.
- Established the golfed minimal-core philosophy (GolfCore, approximately 600–700 bytes).
- Identified a unified entity/composition model and shared physics, fields, constraints and energy mechanisms as the architectural direction.
- Identified declarative chemical and biological rules.
- Identified emergence from particles through protocells and colonies.
- Reviewed the implementation footprint and exposed the estimate-versus-actual discrepancy.
- Investigated the role and lineage of `emergence.js`.
- Requested a golfed, maximally abstracted rewrite/review of the approximately 12k-character implementation.
- Requested consolidation of four areas, followed by another consolidation assessment focused on semantic interoperability, modularisation and abstraction potential.
- Requested further investigation of primitive generalisation, universal abstraction and simplification.
- Requested three further consolidation passes.

The above list distinguishes reported discussion and requests from verified merged implementation. The available project record does not establish that every requested pass has been completed and tested.

## 5. Current completion assessment

| Area | Current assessment |
|---|---|
| Project identity and scope | Established |
| VEPA lineage | Established |
| Boids implementation exclusion | Explicit constraint |
| GolfCore philosophy | Established |
| `accretion.html` as central artifact | Reported project decision |
| Unified substrate architecture | Design scope |
| Shared physics/fields/constraints/energy | Design scope |
| Declarative chemistry/biology | Design scope |
| Particle-to-protocell-to-colony emergence | Design scope |
| Consolidation investigation | In progress / requested iteratively |
| Four-area consolidation | Requested; final verified state unavailable |
| Three additional passes | Requested; completion unverified |
| Current source reconciliation | Outstanding |
| Current tests and CI | Unverified |
| Runtime smoke test | Unverified |
| Current measured size baseline | Outstanding |

## 6. Immediate risks

1. **Competing artifacts:** `emergence.js` and `accretion.html` may describe overlapping implementation generations.
2. **Measurement ambiguity:** the 12,350-character shared-substrate figure and individual artifact counts need a common measurement definition.
3. **Status inflation:** a requested or discussed feature can be mistaken for a completed feature.
4. **Abstraction without proof:** aggressive golfing can obscure semantics or introduce regressions unless behaviour is tested.
5. **Fragmented contracts:** modules can appear modular while still depending on incompatible representations.
6. **Scope contamination:** related project concepts must not become imported code or dependencies.

## 7. Next verification actions

1. Inspect the current authoritative `accretion.html`.
2. Establish whether `emergence.js` is active, superseded or retained only as historical reference.
3. Inventory every primitive, shared mechanism, consumer and duplicated implementation.
4. Re-run character and non-whitespace measurements with a documented counting method.
5. Map every feature to source locations and tests.
6. Run the test suite and report actual results.
7. Run the simulation and perform a runtime smoke test.
8. Update this status file from evidence, not recollection.

## 8. Reporting rule

Every future consolidation report must include:
- Pass number and scope.
- Changes actually made.
- Features or primitives consolidated.
- Semantic and compatibility effects.
- Tests run and results.
- Before and after character counts.
- Before and after non-whitespace counts.
- Any regressions, deferred work or unresolved questions.

Never report a pass as complete merely because an assessment or proposal was written.
