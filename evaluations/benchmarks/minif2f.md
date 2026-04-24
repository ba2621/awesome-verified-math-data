# MiniF2F

**Category:** Benchmarks & Evaluation Sets
**Link:** https://github.com/openai/miniF2F

## Description

488 competition-level math problems (AMC, AIME, IMO, and others) formalized in Lean 4, Lean 3, Isabelle, HOL Light, and Metamath. The standard benchmark for evaluating neural theorem provers on olympiad-style problems.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 3 |
| Level of Formalization | 9 |
| Ease of Use | 9 |
| Complexity | 8 |
| **Overall** | **7.0** |

## Justification

### Data Diversity (6/10)
Covers algebra, number theory, and combinatorics at the competition level, formalized across four proof assistants. Diversity within the competition math domain is good, but the dataset is intentionally narrow — no analysis, topology, or graduate-level mathematics.

### Size (3/10)
Only 488 problems, which is small by dataset standards. However, for a benchmark this is appropriate; the value is in quality and standardization, not volume.

### Level of Formalization (9/10)
All problems are formally stated in multiple proof assistants. Many also have formal proofs (especially for the validation split). The cross-system availability is a notable formalization strength, though not all problems have verified solutions.

### Ease of Use (9/10)
The standard benchmark in the field — every major neural theorem proving paper reports MiniF2F results. Well-documented, has a clear train/test split, and is directly usable with LeanDojo, PISA, and similar frameworks. Extremely accessible.

### Complexity (8/10)
AMC, AIME, and IMO problems require genuine mathematical insight. The problems are hard by any standard, and formal proofs are correspondingly difficult to find. The AIME and IMO subsets represent some of the hardest formally-stated problems available at scale.
