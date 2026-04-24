# Lean Workbook

**Category:** Human-Authored Reference Datasets
**Link:** https://arxiv.org/abs/2406.03847

## Description

Approximately 57,000 informal math problems (primarily competition-style) with corresponding Lean 4 formal statements. Partially verified — some statements have been checked, but the dataset is not uniformly formally proven. Bridges the informal-formal gap at scale.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 7 |
| Size | 7 |
| Level of Formalization | 5 |
| Ease of Use | 7 |
| Complexity | 6 |
| **Overall** | **6.4** |

## Justification

### Data Diversity (7/10)
57,000 problems drawn from competition math sources across algebra, number theory, combinatorics, and geometry. Diverse within the competition math domain and large enough to represent the full range of AMC/AIME-style problems.

### Size (7/10)
57,000 problems is large for a dataset with formal Lean 4 statements. Substantially bigger than MiniF2F or ProofNet, making it a meaningful resource for training models on informal-formal aligned data at scale.

### Level of Formalization (5/10)
Partially verified — formal Lean 4 statements exist for all problems, but not all have been fully proved within Lean. The statement formalization has been checked for syntactic validity, but semantic correctness of the formalization (whether the formal statement captures the informal intent) is not uniformly guaranteed.

### Ease of Use (7/10)
Available through the paper and HuggingFace. Lean 4 statements are accessible with standard tooling. The mixed verification status requires users to filter by proof availability for fully verified subsets.

### Complexity (6/10)
Competition math level — primarily AMC, AIME, and similar. Harder than grade-school or precalculus problems but below graduate-level or IMO difficulty. A solid mid-range complexity dataset.
