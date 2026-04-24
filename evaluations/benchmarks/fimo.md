# FIMO

**Category:** Benchmarks & Evaluation Sets
**Link:** https://arxiv.org/abs/2309.04295

## Description

A dataset of International Mathematical Olympiad (IMO) problems formalized in Lean 4. Provides formal statements for IMO problems, enabling rigorous evaluation of theorem provers on the most difficult competition mathematics.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 3 |
| Size | 2 |
| Level of Formalization | 9 |
| Ease of Use | 7 |
| Complexity | 10 |
| **Overall** | **6.2** |

## Justification

### Data Diversity (3/10)
Exclusively IMO problems. While IMO spans algebra, combinatorics, geometry, and number theory, the narrow source severely limits diversity. This is a deliberate design choice for a targeted evaluation benchmark.

### Size (2/10)
The IMO corpus is inherently small — only ~6 problems per year since 1959, and not all have been formalized. FIMO contains only a subset of these. The dataset is tiny in absolute terms.

### Level of Formalization (9/10)
Problems are formally stated in Lean 4 with care taken to preserve the precise mathematical meaning of each problem. The formalization is high quality even though the proofs themselves are not all formally verified.

### Ease of Use (7/10)
Small and well-defined, making it easy to work with. The Lean 4 statements are available and usable with standard tools. Limited in scope means limited setup overhead.

### Complexity (10/10)
IMO problems are among the hardest competition mathematics problems in the world, selected to challenge the best mathematical minds of each generation. A formal proof of any IMO problem represents a significant achievement. This dataset targets the absolute ceiling of competition math complexity.
