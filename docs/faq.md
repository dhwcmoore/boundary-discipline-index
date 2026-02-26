# FAQ

## Why is this index repo so minimal?
Because it is designed to signal stability and clarity. The index repo is navigation, not an archive.

## Where is the rest of the work?
Some work is private or in progress. It will be released only after it is reorganised into buildable, coherent repositories.

## Why include formal methods and applied modelling together?
Because the technical ambition is not just modelling, but constraint-aware modelling with verification-grade outputs. In AI safety terms: formal specification, interpretable system design, and verifiable output chains are not separate concerns — they are stages of the same discipline.

## What should I review first?

If you are an AI safety researcher or fellowship reviewer:
- read the index README for the AI safety framing and how the work connects to safety research priorities
- read `architecture/repo_map.md` for the per-repo connections to interpretability, control, and oversight
- read `architecture/principles.md` for the design constraints that unify the work
- the Lean and Rocq projects are most directly relevant to formal reasoning about system behaviour; the rupture engine demonstrates interpretable, deterministic system design in a concrete applied setting

If you are a formal methods reviewer:
- start with the Lean library and the Rocq or Coq project

If you are a systems or quant reviewer:
- start with the Rust rupture engine

If you are a hiring manager:
- read the index README and the repo READMEs
- build one repository locally
- skim tests and structure
