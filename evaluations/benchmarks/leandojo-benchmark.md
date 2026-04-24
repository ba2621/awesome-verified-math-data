# LeanDojo Benchmark

**Category:** Benchmarks & Evaluation Sets
**Link:** https://leandojo.org/

## Description

Theorems and proofs extracted from Mathlib4 using the LeanDojo toolkit, with tactic-level annotations, premise retrieval labels, and proof state traces. Designed as a training and evaluation corpus for premise-selection and proof-search models in Lean 4.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 8 |
| Size | 8 |
| Level of Formalization | 10 |
| Ease of Use | 9 |
| Complexity | 7 |
| **Overall** | **8.4** |

## Justification

### Data Diversity (8/10)
Inherits Mathlib4's broad mathematical coverage — algebra, analysis, topology, number theory, and more. Slightly below Mathlib4 itself because the benchmark applies selection and splitting criteria that may under-represent some subfields.

### Size (8/10)
Tens of thousands of theorems with full tactic traces and premise annotations. One of the largest tactic-level formal proof datasets available, enabling training of granular proof step models.

### Level of Formalization (10/10)
All data is extracted directly from Mathlib4, which is fully formally verified. Tactic traces represent actual proof steps accepted by the Lean 4 kernel — no approximation or partial verification.

### Ease of Use (9/10)
Exceptional usability. LeanDojo provides a Python API for interacting with Lean 4 programmatically, pre-extracted datasets in structured formats, and detailed documentation. The de facto standard for training retrieval-augmented theorem provers. Lowers the barrier to entry substantially.

### Complexity (7/10)
Reflects Mathlib4's distribution — predominantly graduate-level but not skewed toward olympiad-style competition problems. Many theorems are specialized results requiring domain knowledge. Slightly lower than Mathlib4 overall because the benchmark split may favor more tractable theorems for fair evaluation.
