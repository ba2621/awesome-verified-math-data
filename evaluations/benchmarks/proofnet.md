# ProofNet

**Category:** Benchmarks & Evaluation Sets
**Link:** https://github.com/zhangir-azerbayev/ProofNet

## Description

A benchmark of undergraduate-level mathematical theorems with formal Lean 4 statements, drawn from textbooks in analysis, algebra, and topology. Designed specifically to evaluate autoformalization — the task of translating informal mathematical statements into formal ones.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 5 |
| Size | 3 |
| Level of Formalization | 8 |
| Ease of Use | 8 |
| Complexity | 6 |
| **Overall** | **6.0** |

## Justification

### Data Diversity (5/10)
Covers real analysis, linear algebra, abstract algebra, and topology at the undergraduate level. Diversity is moderate — the selection reflects standard textbook curricula rather than a broad sweep of mathematical areas.

### Size (3/10)
Small by dataset standards (hundreds of problems). As with MiniF2F, the value is in quality and targeted evaluation rather than volume.

### Level of Formalization (8/10)
Theorem statements are formally stated in Lean 4, but the benchmark is focused on statement formalization rather than complete proof formalization. Many entries lack formal proofs, which limits the training signal for proof search models.

### Ease of Use (8/10)
Clean dataset format, well-described in the accompanying paper, and directly usable for autoformalization evaluation. Paired informal-formal statements make it straightforward to use as a test set.

### Complexity (6/10)
Undergraduate-level mathematics — real analysis (epsilon-delta proofs, continuity), linear algebra (vector spaces, eigenvalues), abstract algebra (groups, rings). Harder than competition arithmetic but not at the research frontier.
