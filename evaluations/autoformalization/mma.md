# MMA (Multilingual Mathematical Autoformalization)

**Category:** Autoformalization Datasets
**Link:** https://arxiv.org/abs/2311.02155

## Description

Informal-formal mathematical pairs across multiple natural languages (English, Chinese, French, etc.) and multiple proof assistants (Lean, Isabelle, Metamath). Designed to study autoformalization as a multilingual and multi-system problem.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 8 |
| Size | 6 |
| Level of Formalization | 7 |
| Ease of Use | 7 |
| Complexity | 6 |
| **Overall** | **6.8** |

## Justification

### Data Diversity (8/10)
The strongest aspect of this dataset. Cross-linguistic coverage (multiple human languages) combined with cross-system coverage (multiple proof assistants) creates a uniquely diverse dataset for studying the general problem of autoformalization beyond English-Lean pairs.

### Size (6/10)
Moderate in size — larger than single-paper artifacts but smaller than large-scale benchmarks. The multilingual dimension means that per-language/system coverage is thinner than a monolingual dataset of equal total size.

### Level of Formalization (7/10)
Informal-formal pairs with formal statements in multiple systems. Not all entries have complete formal proofs; focus is on statement translation. Verification completeness varies by system.

### Ease of Use (7/10)
Well-described in the paper with accessible data format. Useful for multilingual autoformalization research. Standard preprocessing required but not prohibitive.

### Complexity (6/10)
Problems span a range from competition math to undergraduate-level theorems. The multilingual focus means problems were selected for translatability rather than mathematical difficulty, placing the average at a moderate complexity level.
