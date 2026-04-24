# Draft-Sketch-Prove

**Category:** Synthetic & Generated Corpora
**Link:** https://arxiv.org/abs/2210.12283

## Description

A system and dataset that generates proof attempts in a three-stage pipeline: an LLM drafts an informal proof, extracts a formal sketch, and a verifier (Isabelle's Sledgehammer) fills in the remaining steps. The resulting dataset contains informal drafts, formal sketches, and completed verified proofs.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 5 |
| Level of Formalization | 7 |
| Ease of Use | 6 |
| Complexity | 6 |
| **Overall** | **6.0** |

## Justification

### Data Diversity (6/10)
Applied to Isabelle/HOL problems from PISA and MiniF2F. Covers competition math and some Isabelle library theorems. Moderate diversity — constrained by what the pipeline can successfully verify.

### Size (5/10)
Moderate. The pipeline has a non-trivial failure rate, so the verified output is smaller than the attempted input. Dataset size reflects pipeline throughput rather than a comprehensive corpus construction effort.

### Level of Formalization (7/10)
The final proofs are verified by Isabelle/HOL. However, the informal draft and sketch intermediate stages are unverified, and the dataset captures all three stages — so the formalization guarantee applies only to the final step.

### Ease of Use (6/10)
The three-stage format (draft, sketch, proof) is richer than a simple informal-formal pair but requires more preprocessing. Isabelle/HOL dependency adds tooling overhead. The paper provides code but setup is non-trivial.

### Complexity (6/10)
Competition math and Isabelle library theorems — moderately complex. The pipeline is tuned for problems where Sledgehammer can close goals, which biases toward more automatable (and thus somewhat less frontier-difficult) statements.
