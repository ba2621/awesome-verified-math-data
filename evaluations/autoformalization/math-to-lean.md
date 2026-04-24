# MATH-to-Lean

**Category:** Autoformalization Datasets
**Link:** https://github.com/wellecks/ntptutorial

## Description

Datasets and tutorial materials from research on neural theorem proving, including informal-formal pairs that pair competition math problems from the MATH dataset with Lean 4 statements and proofs. Accompanies a tutorial on neural theorem proving methodology.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 5 |
| Level of Formalization | 7 |
| Ease of Use | 7 |
| Complexity | 6 |
| **Overall** | **6.2** |

## Justification

### Data Diversity (6/10)
Covers competition mathematics (MATH dataset problems) formalized in Lean 4. Reasonably diverse within the competition math domain but does not extend to research-level or proof-assistant-native mathematics.

### Size (5/10)
Moderate — draws from a subset of the MATH dataset. Not as large as the full MATH dataset and not all problems have complete formal proofs. Sufficient for methodology research but not for large-scale training.

### Level of Formalization (7/10)
Informal-formal pairs vary in completeness. Some entries have fully verified Lean 4 proofs; others have only formal statements. The mixed verification status is characteristic of this class of autoformalization dataset.

### Ease of Use (7/10)
Distributed with tutorial code and explanatory notebooks, making it accessible for researchers new to neural theorem proving. Clear setup instructions and integration with standard tools.

### Complexity (6/10)
Competition math at the AMC/AIME level — harder than grade school, easier than IMO or graduate research. The formalization adds complexity beyond the informal problem, but the underlying mathematics is at the same level as the MATH dataset.
