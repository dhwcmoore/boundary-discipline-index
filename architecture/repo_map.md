# Repository map

This index points to three primary repositories, each chosen to represent a distinct capability.

## Rust rupture engine (systems + modelling)
Core idea:
- time series are treated as regime-governed behaviour
- rupture is not a vague label but a deterministic state transition
- strain accumulates with long-memory dynamics

Outputs:
- regime classification
- rupture flags
- interpretable internal state transitions

## Lean boundary discipline library (formal foundations)
Core idea:
- boundaries and partitions are formal objects
- composition is treated as an operation with constraints
- topological intuitions are treated carefully and explicitly

Outputs:
- definitional library
- lemmas and theorems about boundary and composition
- a buildable Lean project demonstrating competence and clarity

## VeriBound (Rocq or Coq) with seal (audit-grade verification)
Core idea:
- verification output must be audit-grade
- the output must carry integrity markers that can be recomputed and checked
- the system supports compliance narratives: trace, seal, replay, verify

Outputs:
- structured verification report formats
- seal generation and checking logic
- clear audit-facing framing

## Intended convergence

The long-term integration direction is:

- formal boundary logic provides stable definitions and constraints
- deterministic modelling applies those constraints in applied domains
- audit-grade verification provides integrity and traceability for outputs

This index repo remains the stable navigation layer.
