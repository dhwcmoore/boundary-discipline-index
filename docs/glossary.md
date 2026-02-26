# Glossary

This glossary defines structural terms that recur across the four
repositories. Each term reflects the central thesis: generation must be
constrained by explicit invariants and externally verifiable structure.

------------------------------------------------------------------------

## Audit Layer

An external mechanism that independently recomputes or verifies system
outputs. The audit layer does not trust internal generation and instead
validates artefacts against deterministic rules.

------------------------------------------------------------------------

## Boundary

A formal delimiter separating regions, states, or behavioural phases.
Boundaries prevent silent blending of categories and make transitions
explicit.

------------------------------------------------------------------------

## Closure

The certification or validation of outputs. In this portfolio, closure
is architecturally distinct from production and must not be implicitly
performed by the generating process itself.

------------------------------------------------------------------------

## Deterministic Transition

A state change fully determined by prior state and input. Deterministic
transitions enable exact replay, inspection, and falsifiability.

------------------------------------------------------------------------

## External Verification

Validation performed by a component structurally separate from the
generator. External verification constrains behaviour rather than
deferring to it.

------------------------------------------------------------------------

## Invariant

A property formally specified to hold across all transitions. Invariants
restrict permissible behaviour and reduce drift or silent failure.

------------------------------------------------------------------------

## Long-Memory Accumulation

A cumulative signal that integrates structural strain over extended time
horizons. This reduces sensitivity to noise and emphasises persistent
structural change.

------------------------------------------------------------------------

## Partition Integrity (No Gap / No Overlap)

A constraint ensuring complete coverage and mutual exclusivity of
classifications. Prevents silent omissions or contradictory state
assignments.

------------------------------------------------------------------------

## Production

The component responsible for generating outputs or state labels.
Production is treated as fallible and must remain separate from
verification.

------------------------------------------------------------------------

## Seal

A deterministic integrity marker derived from execution traces. A seal
allows independent recomputation and tamper detection.

------------------------------------------------------------------------

## Structural Separation

The architectural principle that generation, constraint, and
verification must occupy distinct roles. Separation reduces
self-certifying failure modes.

------------------------------------------------------------------------

## Trace Integrity

The guarantee that execution artefacts can be independently recomputed
and checked for consistency. Integrity enables reproducibility and
accountability.
