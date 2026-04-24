# MATH

**Category:** Human-Authored Reference Datasets
**Link:** https://github.com/hendrycks/math

## Description

12,500 competition math problems with step-by-step solutions, spanning 7 subjects (algebra, counting & probability, geometry, intermediate algebra, number theory, prealgebra, precalculus) at 5 difficulty levels. A foundational benchmark for evaluating mathematical reasoning in LLMs.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 7 |
| Size | 6 |
| Level of Formalization | 1 |
| Ease of Use | 9 |
| Complexity | 7 |
| **Overall** | **6.0** |

## Justification

### Data Diversity (7/10)
Seven distinct mathematical subjects with a five-level difficulty scale provides good structural diversity. Coverage is limited to competition mathematics rather than research-level or proof-assistant mathematics, but within that scope the diversity is strong.

### Size (6/10)
12,500 problems is substantial for a curated competition dataset but modest compared to synthetic or automatically generated corpora. The quality and curation effort is high; scale was not the primary goal.

### Level of Formalization (1/10)
Entirely informal. Solutions are in natural language with LaTeX notation. No formal verification has been applied; the data may contain errors, and there is no machine-checkable correctness guarantee. Included here as a reference dataset, not as verified data.

### Ease of Use (9/10)
Extremely well-documented and widely used. Available in standard formats, integrated into every major LLM evaluation framework, and supported by extensive tooling. One of the easiest datasets in this list to work with immediately.

### Complexity (7/10)
Difficulty 5 problems (the hardest level) require genuine competition math skill. The range from prealgebra to precalculus means the dataset spans a wide difficulty spectrum. At the upper end, problems challenge even state-of-the-art LLMs.
