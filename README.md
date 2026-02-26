# Boundary Discipline Index

**Portfolio Map for Deterministic Systems, Formal Kernels, and
Structural AI Safety**

Author: Duston Moore\
Location: Canada\
Focus: Mechanistic Interpretability · Formal Invariants · Deterministic
Architectures

------------------------------------------------------------------------

## Purpose of This Repository

This repository serves as a structured index of core projects exploring
a shared architectural principle:

> Generation processes should not implicitly certify themselves.\
> Verification, constraint, and invariants should be structurally
> explicit.

The repositories linked below demonstrate this principle across
deterministic engines, formally verified kernels, and auditable runtime
systems.

------------------------------------------------------------------------

## Core Repositories

### 1. Rupture Engine

https://github.com/dhwcmoore/rupture-engine

A deterministic rupture detection engine implementing long-memory strain
accumulation and explicit state-machine confirmation.

Key characteristics:

-   Long-memory accumulation of structural strain\
-   Explicit, interpretable state transitions\
-   Deterministic classification logic\
-   No opaque optimisation loop

Although demonstrated on financial time series, the architecture is
domain-agnostic. The engine models structural rupture detection using
explicit dynamics rather than learned heuristics.

Role in portfolio:

Demonstrates interpretable, deterministic modelling where state
transitions are inspectable and reproducible.

------------------------------------------------------------------------

### 2. Verified Yield Regime Kernel

https://github.com/dhwcmoore/verified-yield-regime-kernel

A formally specified threshold-dynamics state-transition kernel with:

-   Invariant proof in Rocq\
-   Mechanical extraction to OCaml\
-   Deterministic runtime execution\
-   JSONL audit trace output

Architecture pattern:

Data → Extracted Kernel → Deterministic State Update → JSONL Trace

Although illustrated using yield curve spread classification, the
architectural contribution is structural: specification is separated
from execution, and invariants are enforced externally rather than
assumed internally.

Role in portfolio:

Demonstrates formal production/closure separation and externally
enforced correctness constraints.

------------------------------------------------------------------------

## Cross-Cutting Theme

Across these systems:

-   State transitions are explicit.
-   Invariants are defined rather than assumed.
-   Execution is deterministic and auditable.
-   Verification is external to generation.

This architectural framing motivates ongoing empirical work in
mechanistic interpretability. If neural systems collapse generation and
verification internally, measurable structural signatures may exist in
their representations.

------------------------------------------------------------------------

## Relevance to AI Safety Research

These repositories collectively explore:

-   Structural separation of roles
-   Deterministic traceability
-   External constraint enforcement
-   Interpretable state-machine dynamics

They serve as concrete system-level analogues for research questions in:

-   Mechanistic interpretability\
-   Scalable oversight\
-   Robustness under distribution shift

This index functions as a structured map of that work.
