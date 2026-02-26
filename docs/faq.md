# FAQ

This FAQ clarifies the architectural intent of the four-repository
stack.

------------------------------------------------------------------------

## What is the unifying idea behind these projects?

Powerful systems should not implicitly certify their own outputs.
Structural constraints and verification must be explicit, external, and
reproducible.

------------------------------------------------------------------------

## Why prioritise deterministic systems?

Determinism allows exact replay and inspection. Claims about behaviour
can be tested and falsified without relying on probabilistic
explanations.

------------------------------------------------------------------------

## Why combine formal proofs with executable engines?

Proof artefacts constrain what the system is allowed to do. Executable
engines demonstrate how those constraints behave in practice. The
combination models specification bounding generation.

------------------------------------------------------------------------

## Why include a separate sealing or verification layer?

Execution artefacts should be independently checkable. A separate
verification layer reduces the risk of undetected modification or silent
failure.

------------------------------------------------------------------------

## Are these domain-specific tools?

The example domains are illustrative. The architectural
principles---explicit transitions, invariant preservation, and external
verification---are domain-agnostic.

------------------------------------------------------------------------

## How do the four repositories form a stack?

1.  Deterministic modelling (rupture-engine)\
2.  Formally specified invariant kernel (verified-yield-regime-kernel)\
3.  Structural boundary reasoning (boundary-discipline-lean)\
4.  External trace integrity (veribound-rocq-seal)

Each layer constrains the next, reinforcing structural separation.

------------------------------------------------------------------------

## How does this connect to interpretability and oversight research?

These repositories model how generation can be bounded by explicit
constraints and independent verification. Similar structural questions
arise when analysing internal representations of large models: whether
roles are separable, whether invariants persist, and whether
verification is external or implicit.

------------------------------------------------------------------------

## Are these production systems?

No. They are minimal, controlled artefacts designed to illustrate
architectural constraints clearly and reproducibly.
