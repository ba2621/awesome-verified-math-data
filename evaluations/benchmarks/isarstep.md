# ISARSTEP

**Category:** Benchmarks & Evaluation Sets
**Link:** https://github.com/Wenchichang/ISARSTEP

## Description

A benchmark for high-level mathematical reasoning in Isabelle, constructed by extracting step-level proof transitions from the Archive of Formal Proofs (AFP). Each example consists of a proof state (hypotheses and goal) and the next human-written tactic step, enabling training and evaluation of step-level proof prediction models. Associated paper: [arxiv.org/abs/2006.09265](https://arxiv.org/abs/2006.09265).

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 8 |
| Level of Formalization | 10 |
| Ease of Use | 5 |
| Complexity | 7 |
| **Overall** | **7.2** |

## Justification

### Data Diversity (6/10)
Sourced from the AFP, which spans algebra, analysis, number theory, combinatorics, and more. However, the step-level extraction focuses on Isabelle/HOL tactic structure, so the perspective is narrower than the AFP's full breadth. All data is Isabelle-only.

### Size (8/10)
Tens of thousands of proof step examples extracted from thousands of AFP theories. The step-level granularity means each theorem contributes many training examples, making the effective dataset size substantially larger than theorem-count alone would suggest.

### Level of Formalization (10/10)
Every proof step is sourced directly from the AFP, which is fully machine-verified by Isabelle. Each tactic step has been executed successfully; there are no unverified or speculative proof steps in the corpus.

### Ease of Use (5/10)
Requires an Isabelle/HOL environment to interact with the data at the proof-state level. The Isabelle ecosystem has steeper setup requirements than Lean 4, and tooling for programmatic interaction (e.g. PISA) is less mature than LeanDojo. The step-level format is well-specified but unfamiliar to researchers primarily working in Lean.

### Complexity (7/10)
AFP content spans undergraduate to graduate-level mathematics. The step-level format presents a different kind of difficulty than problem-level benchmarks: the challenge is predicting the correct next tactic given a proof state, which requires both mathematical understanding and knowledge of Isabelle's tactic language.
