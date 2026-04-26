# PutnamBench

**Category:** Benchmarks & Evaluation Sets
**Link:** https://github.com/trishullab/PutnamBench

## Description

640+ William Lowell Putnam Mathematical Competition problems (spanning 1962–2023) formalized in Lean 4 and Isabelle. Putnam problems represent some of the hardest undergraduate competition mathematics — routinely requiring graduate-level insight — making this the highest-complexity benchmark in the formal math ecosystem. Associated paper: [arxiv.org/abs/2407.11214](https://arxiv.org/abs/2407.11214).

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 5 |
| Size | 3 |
| Level of Formalization | 9 |
| Ease of Use | 7 |
| Complexity | 10 |
| **Overall** | **6.8** |

## Justification

### Data Diversity (5/10)
Covers calculus, real analysis, algebra, combinatorics, number theory, and probability — the standard Putnam topics — formalized across two proof assistants. Diversity within the Putnam domain is reasonable, but the dataset is intentionally narrow to competition problems; no topology, category theory, or formal library-style breadth.

### Size (3/10)
640 problems is small in absolute terms, comparable to MiniF2F. As with MiniF2F, the value is in quality and difficulty rather than volume. Each formalization represents significant manual effort given Putnam problem complexity.

### Level of Formalization (9/10)
Problems are formally stated (and in some cases proven) in Lean 4 and Isabelle. Cross-system coverage is a strength shared with MiniF2F. Not all entries have complete formal proofs — the benchmark primarily tests statement-level formalization and proof search.

### Ease of Use (7/10)
Well-documented GitHub repository with clear problem indexing by year and number. The dual Lean 4 / Isabelle availability makes it usable by researchers in either ecosystem. Requires a working Lean 4 or Isabelle setup, but no custom tooling beyond the standard proof assistant infrastructure.

### Complexity (10/10)
Putnam problems are uniquely difficult — they require mathematical creativity that goes well beyond their ostensibly undergraduate scope. Formal proofs of Putnam problems represent the frontier of what neural theorem provers can attempt. No other publicly available formalized benchmark matches this difficulty ceiling.
