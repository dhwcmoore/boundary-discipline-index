# Boundary Discipline Index

**Portfolio: Deterministic Architectures, Formal Invariants, and
External Verification**

Author: Duston Moore
Location: Canada
Focus: Mechanistic Interpretability · Structural Invariants · Oversight
Architectures

------------------------------------------------------------------------

## Architectural Thesis

Powerful systems should not be trusted to certify their own behaviour.

Generation, constraint, and verification must remain structurally
distinct roles.
Invariants should be explicit rather than implicit.
State transitions should be inspectable rather than opaque.
Execution should produce artefacts that can be independently recomputed
and verified.

The four pinned repositories below are small, buildable artefacts that
instantiate this architectural stance across deterministic engines,
formal kernels, and audit layers.

They are designed as system-level analogues for questions that arise in
interpretability and oversight research: how structural guarantees can
bound behaviour without relying on internal self-certification.

------------------------------------------------------------------------

## The Stack

### 1) Rupture Engine (Rust)

https://github.com/dhwcmoore/rupture-engine

A deterministic rupture detection engine based on long-memory strain
accumulation and explicit state-machine confirmation.

Characteristics:

-   Explicit state transitions
-   Deterministic regime emission
-   Long-memory accumulation rather than transient thresholding
-   Structured output logs for replay and inspection

Role in the stack:

Models interpretable behavioural emergence under accumulated structural
stress. Demonstrates how classification logic can remain transparent and
reproducible without relying on opaque optimisation.

------------------------------------------------------------------------

### 2) Verified Yield Regime Kernel (Rocq → OCaml)

https://github.com/dhwcmoore/verified-yield-regime-kernel

A formally specified state-transition kernel with a proved invariant in
Rocq, mechanically extracted to OCaml and executed deterministically
with JSONL trace output.

Characteristics:

-   Proven regime invariant
-   Mechanical extraction preserving specification
-   Deterministic runtime behaviour
-   Structured audit trace

Role in the stack:

Demonstrates production/closure separation. The specification constrains
the executable artefact rather than emerging from it.

------------------------------------------------------------------------

### 3) Boundary Discipline (Lean)

https://github.com/dhwcmoore/boundary-discipline-lean

A Lean 4 + mathlib formalisation of regions, partitions, and boundary
operators, including preservation results under composition and
refinement.

Characteristics:

-   Explicit coverage constraints (no gap / no overlap)
-   Boundary operators as first-class objects
-   Preservation theorems under composition

Role in the stack:

Provides the mathematical substrate for reasoning about structural
completeness and invariant preservation.

------------------------------------------------------------------------

### 4) VeriBoundand Seal (Rocq → OCaml)

https://github.com/dhwcmoore/veribound-rocq-seal

A narrow, buildable slice of an audit-grade sealing system that couples
formal artefacts with deterministic trace integrity checks.

Characteristics:

-   Deterministic seal recomputation
-   Tamper detection
-   Minimal verifier for runtime artefacts

Role in the stack:

Adds external verification. Execution outputs can be independently
recomputed and checked for integrity.

------------------------------------------------------------------------

## Emergent Architecture

Taken together, the four repositories form a layered safety analogue:

Deterministic modelling
→ Formal invariants
→ Structural partition guarantees
→ Independent audit and verification

Each layer constrains the next.

The combined effect is stronger than any single component: behavioural
modelling is bounded by invariants, invariants are grounded in formal
reasoning, and outputs are externally verifiable.

------------------------------------------------------------------------

## Relevance to Empirical Safety Research

These projects are not large-scale models. They are minimal, controlled
artefacts designed to explore structural questions relevant to:

-   Mechanistic interpretability
-   Oversight mechanisms
-   Robustness under distribution shift
-   Separation of generation and verification roles

The research trajectory extends these architectural principles toward
empirical investigation of internal model representations, where
structural collapse or role conflation may be measurable rather than
assumed.

------------------------------------------------------------------------

## Status

All repositories are buildable and self-contained. They prioritise
clarity, determinism, and inspectability over scale.

This index serves as a structured map of that work.
