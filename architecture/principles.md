# Principles

These principles constrain the work across the curated repositories.

## 1) Determinism where possible
When a system can be expressed as an explicit state machine with auditable transitions, prefer that over opaque heuristics.

## 2) Explicit boundaries
If a boundary is being used, it must be defined, not implied. If a partition is assumed, it must be named and checked.

## 3) No gap, no overlap
Whenever possible, represent classifications or partitions so that coverage is complete and ambiguity is minimised.

## 4) Buildable artefacts
A public repository must build. If it cannot build, it is not ready for publication.

## 5) Traceable outputs
Where outputs have compliance or audit relevance, produce structured logs and integrity markers that allow replay and independent checking.

## 6) Minimal, curated surface area
Public work should be narrow and legible. Complexity belongs inside the project, not in the public-facing structure.
