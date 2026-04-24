# Lean Math Formal Corpus

**Category:** Benchmarks & Evaluation Sets
**Link:** https://huggingface.co/datasets/iiis-lean/lean-math-formal-corpus

## Description

A curated corpus of 2,880 formally verified Lean 4 proofs of competition-level mathematics problems from IMO, APMO, EGMO, and other olympiad sources, supplemented by textbook corpora (CombiBench, HackMath, Brualdi). Each entry provides a natural language problem and proof alongside a formally verified Lean 4 theorem and proof, with compile validation and repair-tracking metadata. Associated with five ArXiv papers from Tsinghua IIIS.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 5 |
| Size | 3 |
| Level of Formalization | 10 |
| Ease of Use | 7 |
| Complexity | 9 |
| **Overall** | **6.8** |

## Justification

### Data Diversity (5/10)
Combinatorics is heavily dominant given the olympiad sourcing, with additional coverage of discrete math, graph theory, number theory, geometry, and set theory. Ten source datasets are aggregated, which adds some breadth, but the corpus skews toward discrete and competition mathematics rather than the full spectrum of graduate-level mathematics.

### Size (3/10)
2,880 examples is small. The quality is exceptional (see Formalization score), but the scale limits its utility for large-scale training. More valuable as a benchmark or evaluation set than as a pretraining corpus.

### Level of Formalization (10/10)
All proofs are compile-validated against Lean 4 (supporting versions 4.9.0, 4.15.0, and 4.27.0). The dataset tracks `compile_success`, `theorem_repairs`, and `proof_repairs`, making the verification process auditable. This is the highest standard of formal verification available.

### Ease of Use (7/10)
Well-structured JSONL with both natural language and formal fields, making it immediately usable for autoformalization research. Multiple Lean version fields help with compatibility. The relatively small size keeps loading trivial.

### Complexity (9/10)
IMO, APMO, and EGMO problems are among the hardest mathematics problems that have been formally verified at scale. These require non-trivial proof strategies and represent genuine mathematical research difficulty in the olympiad domain.
