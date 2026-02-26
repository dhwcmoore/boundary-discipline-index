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

AI safety relevance:
- demonstrates that complex system behaviour can be made fully interpretable by construction: every state is named, every transition is explicit, every decision is traceable
- the design philosophy — explicit state machines over opaque heuristics — is directly relevant to AI control and to building systems whose behaviour can be predicted and audited

## Lean boundary discipline library (formal foundations)
Core idea:
- boundaries and partitions are formal objects
- composition is treated as an operation with constraints
- topological intuitions are treated carefully and explicitly

Outputs:
- definitional library
- lemmas and theorems about boundary and composition
- a buildable Lean project demonstrating competence and clarity

AI safety relevance:
- formal methods are the foundation of mechanistic interpretability: specifying what a module computes, not just observing its outputs
- the partition and boundary framework provides mathematical tools for complete, non-overlapping behavioural specifications — directly applicable to formalising properties of AI systems

## VeriBound (Rocq or Coq) with seal (audit-grade verification)
Core idea:
- verification output must be audit-grade
- the output must carry integrity markers that can be recomputed and checked
- the system supports compliance narratives: trace, seal, replay, verify

Outputs:
- structured verification report formats
- seal generation and checking logic
- clear audit-facing framing

AI safety relevance:
- scalable oversight requires output chains that can be independently verified, not just trusted
- cryptographic sealing and structured traces provide the architecture for AI outputs that resist tampering and support post-hoc auditing
- the replay-and-verify model directly addresses the problem of confirming AI system behaviour without re-running the original process

## Verified yield regime kernel (end-to-end formal correctness pipeline)
Core idea:
- formal specification and execution are not separate concerns — they should be connected by mechanical extraction
- a proved invariant is only useful if it applies to the actual running code, not just the abstract model
- audit traces must be structured and deterministic to support independent verification

Outputs:
- Rocq formal specification and proved regime invariant
- mechanically extracted OCaml code (Rocq extraction)
- deterministic runtime with JSONL audit traces
- CI/CD regression test suite

AI safety relevance:
- this repo is the clearest demonstration that formal correctness guarantees can be carried through to a running system — the proved invariant holds not just in the model but in the extracted executable
- the core soundness property ("if step s o emits regime r, then the necessary condition defining r holds for o") is exactly the kind of guarantee that matters for AI control: the system cannot exhibit labelled behaviour without satisfying its formal definition
- mechanical extraction eliminates the implementation gap — a common failure mode where a verified model and its implementation diverge
- structured JSONL audit traces with deterministic runtime directly support scalable oversight: outputs can be replayed, checked, and audited independently

## Intended convergence

The long-term integration direction is:

- formal boundary logic provides stable definitions and constraints
- deterministic modelling applies those constraints in applied domains
- audit-grade verification provides integrity and traceability for outputs
- end-to-end extraction pipelines close the gap between formal models and running code

The verified yield regime kernel is the closest existing realisation of this convergence: it combines formal specification, a proved invariant, mechanical extraction, and deterministic audit-traced execution in a single working project.

In AI safety terms: formal specification → interpretable system design → verifiable output chains → provably correct execution.

This index repo remains the stable navigation layer.
