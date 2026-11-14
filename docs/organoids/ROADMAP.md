# Organoids Roadmap

**Planning snapshot:** 14 November 2026  
**Ordering:** evidence and architectural integrity before feature expansion.

## Phase 1: Establish the real baseline

- [ ] Inspect current `accretion.html`.
- [ ] Locate and classify `emergence.js`.
- [ ] Establish the canonical source-of-truth arrangement.
- [ ] Inventory all current primitives and consumers.
- [ ] Record exact character and non-whitespace counts.
- [ ] Identify test commands, test coverage and current CI state.
- [ ] Run a baseline runtime smoke test.

**Exit condition:** a source-backed inventory with reproducible measurements and a verified baseline.

## Phase 2: Reconcile feature implementation

- [ ] Map each feature in FEATURES.md to source locations.
- [ ] Label each as implemented, partial, planned, obsolete or unverified.
- [ ] Map tests to features.
- [ ] Identify duplicated mechanisms and incompatible data contracts.
- [ ] Correct documentation to reflect actual implementation.

**Exit condition:** no feature is described as complete without implementation and verification evidence.

## Phase 3: Consolidation and abstraction

Continue the requested consolidation programme, including the four-area consolidation work and subsequent assessments.

Focus areas:
- [ ] Semantic interoperability.
- [ ] Modularisation opportunities.
- [ ] Primitive generalisation.
- [ ] Universal abstraction where genuinely useful.
- [ ] Simplification and removal of redundant representations.
- [ ] Shared contracts across physics, fields, constraints and energy.
- [ ] Declarative rule reuse.
- [ ] Elimination of competing implementations.

For every pass, publish the changes and before/after character counts, including non-whitespace counts.

**Exit condition:** measurable reduction in duplication/complexity without semantic regressions.

## Phase 4: Stabilise the substrate

- [ ] Specify GolfCore's exact contract.
- [ ] Specify the canonical entity/composition representation.
- [ ] Specify shared interaction and transformation semantics.
- [ ] Specify rule evaluation and state transition contracts.
- [ ] Add tests for each primitive and cross-module interoperability.
- [ ] Verify deterministic or explicitly stochastic behaviour as appropriate.

**Exit condition:** stable, tested primitives that can support higher-order organisation.

## Phase 5: Demonstrate emergence

- [ ] Demonstrate particle-level interactions.
- [ ] Demonstrate formation of structures and compounds.
- [ ] Demonstrate protocell-like organisation.
- [ ] Demonstrate higher-order organism/colony organisation.
- [ ] Record the mechanisms and rules responsible for each transition.
- [ ] Test that emergence is produced by the general substrate rather than a hidden scripted shortcut.

**Exit condition:** reproducible demonstrations of the intended emergence ladder.

## Phase 6: Delivery and maintenance

- [ ] Confirm CI on the current authoritative branch.
- [ ] Run runtime and regression checks.
- [ ] Document setup and execution.
- [ ] Keep feature and status documents current.
- [ ] Record each completed consolidation pass and its measurements.

## Priority rule

Do not expand the feature catalogue merely to make it longer. First make the existing substrate smaller, more general, interoperable and verifiably correct. Add higher-order capabilities when the substrate can express them cleanly.
