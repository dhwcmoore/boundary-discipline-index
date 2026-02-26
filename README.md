# Boundary Discipline Index

**Empirical Research Portfolio for AI Safety & Interpretability**

**Author:** Duston Moore
**Location:** Canada
**Focus:** Mechanistic Interpretability · Formal Invariants · Structural
AI Safety

------------------------------------------------------------------------

## Overview

This repository documents a research programme exploring a central
question in AI safety:

> Can highly capable models internally certify their own outputs, or is
> external structural oversight necessary?

This work investigates structural failure modes in generative systems
using a combination of:

-   Formal invariants
-   Boundary-based reasoning
-   Lightweight empirical probes
-   Mechanistic interpretability techniques

The goal is to bridge formal verification intuitions with empirical
large-model analysis.

------------------------------------------------------------------------

## Research Motivation

Modern frontier models exhibit increasing autonomy, reasoning depth, and
internal complexity. As capability scales, so does the risk of:

-   Implicit self-certification
-   Representational collapse
-   Hidden optimisation objectives
-   Internal circuit behaviour that diverges from declared outputs

This project studies structural properties of models that may correlate
with these risks.

Rather than treating safety as a behavioural overlay, this research
explores whether safety must instead rely on structural separation
between:

-   **Production** --- the generative process
-   **Closure** --- the verification or certification of outputs

This separation can be studied empirically using interpretability tools.

------------------------------------------------------------------------

## Research Direction

The current focus is on:

### 1. Structural Probes of Internal Representations

Investigating whether internal representations exhibit:

-   Boundary collapse
-   Overcompression of semantic distinctions
-   Internal feature entanglement

### 2. External Verification Analogues

Drawing inspiration from formal verification kernels, this work explores
whether models demonstrate identifiable patterns when:

-   Certifying their own reasoning chains
-   Justifying outputs
-   Performing self-evaluation tasks

### 3. Experimental Approach

Planned empirical methods include:

-   Activation patching
-   Feature attribution
-   Circuit tracing
-   Representation similarity metrics
-   Controlled perturbation experiments

All experiments are designed to be lightweight, reproducible, and
compatible with open-source LLM infrastructure.

------------------------------------------------------------------------

## Technical Background

The research direction builds on prior work in:

-   Lean / Rocq / Coq formal verification
-   Type-level invariants
-   Kernel-based closure systems
-   Deterministic state modelling

This background informs the hypothesis that internal self-certification
without structural separation may produce identifiable empirical
signatures.

------------------------------------------------------------------------

## Why This Matters

If models implicitly collapse production and verification processes,
this may:

-   Reduce reliability under distribution shift
-   Increase vulnerability to adversarial prompts
-   Create alignment fragility at scale

Understanding whether and how such collapse manifests internally could
inform:

-   Interpretability-driven oversight
-   Safer training objectives
-   Structural interventions

------------------------------------------------------------------------

## Intended Output

The aim of this project is to produce:

-   A small empirical study
-   Reproducible experiments
-   Public write-up or paper submission

This repository functions as a structured foundation for that work.

------------------------------------------------------------------------

## Research Intent

I am motivated by reducing catastrophic risks from advanced AI systems
and am transitioning into full-time empirical AI safety research.

I am particularly interested in contributing to:

-   Mechanistic Interpretability
-   Scalable Oversight
-   Structural Approaches to AI Control
