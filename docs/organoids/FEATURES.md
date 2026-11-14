# Organoids Feature Catalogue

**Snapshot:** 14 November 2026

This catalogue separates the intended feature set from implementation evidence. A feature appearing here does not automatically mean it exists in working code.

### Status vocabulary

- **Design scope:** part of the agreed architectural direction.
- **Reported:** previously described as present or implemented, but not independently rechecked against current source.
- **In progress:** actively being consolidated, designed or integrated.
- **Unverified:** discussed or intended; no sufficient implementation evidence is available here.
- **Blocked / unresolved:** requires a decision, integration or verification step.

## 1. Foundational substrate

| Capability | Description | Evidence status |
|---|---|---|
| GolfCore | Minimal functional foundation, approximately 600–700 bytes as a design target/philosophy | Design scope |
| Entity representation | Unified representation for simulation entities | Design scope |
| Composition model | Entities/structures composed from common primitives | Design scope |
| Shared substrate | Common mechanisms rather than isolated feature implementations | Design scope; size discrepancy measured |
| Fields | Shared environmental or interaction fields | Design scope |
| Constraints | General constraints applicable across entity types | Design scope |
| Energy engines | Shared energy-related mechanisms | Design scope |
| Interoperable modules | Modules sharing compatible semantics and representations | Design scope |

## 2. Physics and interactions

- Particle-level representation and interaction.
- Shared physics mechanisms.
- Density, pressure and other interaction properties where required by the chosen physical model.
- Fields that influence entity behaviour and state.
- Constraints governing interactions and permitted transformations.
- Energy transfer and transformation mechanisms.
- Reusable interaction rules rather than per-species physics.

**Evidence:** physics, fields, constraints and energy engines have been identified as shared architectural capabilities. Current numerical models, solver completeness and runtime behaviour are unverified.

## 3. Chemistry and transformation

- Declarative chemical rules.
- General transformation/reaction mechanisms.
- Composition and decomposition.
- Interaction-driven formation of more complex structures.
- Reusable rules for state transitions.
- Shared substrate support for non-living and living structures.

**Evidence:** declarative chemical and biological rules were part of the previously stated feature scope. Specific reaction catalogues and tested reaction behaviour are unverified.

## 4. Biological emergence

- Emergence from particles into structures.
- Compound and protocell formation.
- Organism-like organisation.
- Colony formation.
- Self-organisation through local interactions.
- Growth and structural change.
- Reproduction and propagation as higher-order mechanisms.
- Life-like behaviour arising from shared rules.

**Evidence:** particle-to-protocell-to-colony emergence is established design scope. The completeness of each stage is not verified.

## 5. Higher-order behaviour and ecology

The architecture is intended to permit:
- Autonomous behaviour arising from entity state and interactions.
- Competition and cooperation.
- Resource and energy relationships.
- Population-level dynamics.
- Adaptation through changing structures or rules.
- Interactions between organisms and their environment.

These are capability targets, not a verified checklist of finished simulation features. Detailed ecology, genetics, neural control and population mechanics must be added only where supported by the Organoids architecture and independently implemented.

## 6. Observability and verification

- Tests for foundational primitives.
- Tests for composition and interoperability.
- Tests for transformation and emergence.
- Runtime inspection of simulation state.
- Measured source-size reporting.
- Before/after character counts for consolidation work.
- Regression checks after abstraction changes.

Tests and documentation artifacts were included in the historical size measurements, but their present contents and coverage have not been independently inspected.

## 7. Engineering and delivery

- Single coherent implementation.
- Consolidation of overlapping mechanisms.
- Progressive golfing and abstraction.
- Feature documentation.
- Automated tests and CI.
- Runtime verification.
- Reproducible measurements.

A prior project summary reported a feature branch with CI passing. That historical report must not be treated as confirmation of the current branch or current CI state.

## 8. Explicit exclusions

- Real-world biological organoid development or experimentation.
- Importing Boids implementation, source, dependencies or code.
- Folding Mocean or NEXUS Aquarium into this repository.
- Treating conceptual discussion as proof of implementation.
- Adding specialised subsystems when an existing general primitive can express the behaviour.

## 9. Feature completion rule

A feature should only be marked **complete** when:
1. Its implementation exists in the authoritative source.
2. Its contract and semantics are documented.
3. Relevant tests pass.
4. Integration with the shared substrate is demonstrated.
5. Any runtime-dependent behaviour has been smoke-tested.

Until then, retain the appropriate weaker status.
