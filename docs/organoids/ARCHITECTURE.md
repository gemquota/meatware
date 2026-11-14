# Organoids Architecture

**Status:** intended architecture reconstructed from project discussion; implementation mapping pending source verification.

## 1. Architectural objective

Create one coherent substrate capable of representing and evolving multiple levels of organisation. Avoid separate, bespoke systems for particles, compounds, cells, organisms and colonies when common primitives can express them.

## 2. Conceptual layers

### A. Minimal functional core

GolfCore is the minimal foundational mechanism, with an approximately 600–700-byte target/philosophy. It should establish the smallest useful set of operations and contracts from which the rest of the system can be composed.

The target is not a mandate to cram all functionality into the core. Higher-level capabilities should remain composable extensions.

### B. Entity and composition model

A unified entity/composition model should provide a common representation for the things participating in the simulation.

The model should support:
- Identity and state.
- Composition from smaller entities or components.
- Relationships and interactions.
- State transitions.
- Reuse across physical, chemical and biological contexts.

Exact fields and storage representation require confirmation against `accretion.html`.

### C. Shared physical substrate

Physics, fields, constraints and energy engines should be general mechanisms shared by entities and structures.

Avoid implementing separate physics engines for each emergent level unless a demonstrated semantic or performance requirement justifies it.

### D. Declarative rules

Chemical and biological behaviour should be expressed through declarative rules operating on shared representations.

Rules should describe conditions, interactions and transformations rather than hard-code every possible structure or organism.

### E. Emergent organisation

Higher-order structures should arise from lower-level entities and rules:

`particles → structures → compounds → protocells → organisms → colonies`

Each transition should be explainable through shared composition, interactions, constraints, energy and rule evaluation.

## 3. Interoperability requirements

Modules should agree on:
- Entity identity and references.
- State representation.
- Units and numerical conventions.
- Field and constraint semantics.
- Interaction and transformation contracts.
- Lifecycle and ownership rules.
- Event/observation semantics where used.

A module is not truly interoperable merely because it can call another module's function. It must interpret shared data in the same way.

## 4. Consolidation strategy

For each repeated mechanism:

1. Find all implementations and consumers.
2. Identify the invariant semantics.
3. Define the smallest general primitive that preserves those semantics.
4. Move consumers to the shared primitive.
5. Remove obsolete duplication.
6. Test old and new behaviour.
7. Measure the result.

Prefer abstractions that eliminate multiple kinds of duplication at once. Avoid abstraction layers that merely rename a single-use function or add indirection without improving semantic reuse.

## 5. Golfing strategy

Golfing is a design instrument:
- Compress repeated syntax and operations.
- Generalise repeated structures.
- Remove redundant state.
- Reduce unnecessary control paths.
- Prefer compositional rules over special cases.

Do not optimise character count at the expense of correctness, determinism where required, debuggability or a stable contract. Record both raw and non-whitespace character counts.

## 6. Source-of-truth policy

Project discussion names `accretion.html` as the central artifact. The relationship to historical `emergence.js` must be resolved explicitly.

The desired end state is a single coherent architecture, not two competing implementations. Historical code may inform analysis, but should not silently become a dependency or parallel source of truth.

## 7. Open architecture questions

- What exact operations constitute GolfCore?
- What is the canonical entity schema?
- Which state belongs to entities versus shared fields or engines?
- How are rules represented, evaluated and ordered?
- How are transformations and composition made safe?
- What are the invariants for energy and physical quantities?
- Which mechanisms are genuinely universal and which should remain specialised?
- What is the smallest useful module boundary?
- How is emergence observed and tested without encoding the desired outcome?

Resolve these questions by inspecting the current source and tests, not by inventing a schema from this document.
