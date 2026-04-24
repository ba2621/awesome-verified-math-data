# mathematic-coq

**Category:** Benchmarks & Evaluation Sets
**Link:** https://huggingface.co/datasets/Pawitt/mathematic-coq

## Description

A dataset of 6,207 Coq proof examples drawn from the Mathematical Components library, structured as context–claim–proof triples. The `context` field includes all necessary Coq imports and definitions (up to 300KB), the `claim` field gives the mathematical statement being proved, and the `proof` field contains the formal Coq proof. Covers analysis, number theory, algebra, ordering relations, and norm theory.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 4 |
| Size | 4 |
| Level of Formalization | 9 |
| Ease of Use | 4 |
| Complexity | 6 |
| **Overall** | **5.4** |

## Justification

### Data Diversity (4/10)
Scoped to MathComp's mathematical coverage: analysis, number theory, algebra, and related areas. Does not span the broader landscape of formal mathematics. The domain range is narrower than AFP, Mathlib, or even Coq-MathComp.

### Size (4/10)
6,207 examples is modest. Smaller than Coq-MathComp (which covers more of the library) and much smaller than Lean-based equivalents. Useful for targeted training but not for large-scale experiments.

### Level of Formalization (9/10)
All proofs are drawn from the formally verified MathComp library and include the full Coq proof text. One point below 10 because the dataset provides no explicit compile-success field — correctness is implied by MathComp provenance but not verified at extraction time.

### Ease of Use (4/10)
Very limited documentation and minimal download history (1 download). The large `context` fields (up to 319KB per row) create practical loading challenges. No tooling or example notebooks are provided. The data format is sound but the onboarding experience is poor.

### Complexity (6/10)
MathComp proofs represent solid graduate-level mathematics, but the per-claim complexity is library-style rather than olympiad-style. Individual lemmas tend to be well-scoped rather than deep standalone results.
