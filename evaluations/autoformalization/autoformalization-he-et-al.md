# AutoFormalization with LLMs (He et al.)

**Category:** Autoformalization Datasets
**Link:** https://arxiv.org/abs/2205.12615

## Description

Dataset from early foundational work (2022) on using large language models to translate informal mathematics into formal Lean statements. One of the first systematic studies of LLM-driven autoformalization, pairing informal statements with Lean formal equivalents.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 5 |
| Size | 4 |
| Ease of Use | 6 |
| Level of Formalization | 7 |
| Complexity | 5 |
| **Overall** | **5.4** |

## Justification

### Data Diversity (5/10)
Covers a range of informal mathematical statements from competition and textbook sources, but the scope is bounded by what was feasible to formalize with early LLMs. Moderate topical variety.

### Size (4/10)
A research paper artifact — the dataset is small by modern standards, reflecting the exploratory nature of this early work. Useful as a reference or starting point rather than a training corpus.

### Level of Formalization (7/10)
Informal-formal pairs where formal statements are in Lean. Formalization quality is mixed — some statements are fully verified, others are approximate. As a pioneering effort, the formalization methodology was less rigorous than later work.

### Ease of Use (6/10)
Available as a research artifact alongside the paper. Documentation is adequate but not as polished as later datasets. Requires familiarity with the paper to use effectively.

### Complexity (5/10)
The problems are drawn from accessible informal mathematics to test the feasibility of autoformalization — not selected for mathematical difficulty. Moderate complexity level appropriate for a proof-of-concept study.
