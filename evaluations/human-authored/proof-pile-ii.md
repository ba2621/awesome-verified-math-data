# Proof Pile II / AlgebraicStack

**Category:** Human-Authored Reference Datasets
**Link:** https://huggingface.co/datasets/EleutherAI/proof-pile-2

## Description

A 55-billion-token pretraining corpus for mathematical language models, assembled by EleutherAI. The **AlgebraicStack** subset (~11B tokens) is the formal-math slice: code extracted from public GitHub repositories in Lean, Coq, Isabelle, Agda, Metamath, and other proof assistants. The remainder includes mathematical arXiv papers and curated web content. Used to train several open-source math LMs. Associated paper: [arxiv.org/abs/2310.10631](https://arxiv.org/abs/2310.10631).

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 9 |
| Size | 10 |
| Level of Formalization | 3 |
| Ease of Use | 8 |
| Complexity | 7 |
| **Overall** | **7.4** |

## Justification

### Data Diversity (9/10)
Spans formal proof code (Lean, Coq, Isabelle, Agda, Metamath), mathematical arXiv papers across nearly every subfield, and supplementary web content. The AlgebraicStack alone covers every major proof assistant. Breadth across formalism, language, and mathematical domain is unmatched in this list.

### Size (10/10)
55 billion tokens — by far the largest corpus here by token count. The AlgebraicStack formal-code slice alone exceeds 11B tokens, dwarfing all other formal math datasets combined. Designed explicitly for continued pretraining of large language models.

### Level of Formalization (3/10)
The majority of the corpus (arXiv papers, web math) is informal and unverified. The AlgebraicStack slice contains formal proof code sourced from public repositories, but not all of it compiles or constitutes verified proofs — repositories may contain work in progress, broken proofs, or tactic skeletons. A score above 1 reflects that the formal code slice is meaningful, but this dataset cannot be treated as a verified corpus.

### Ease of Use (8/10)
Available directly on HuggingFace in a standard format. EleutherAI provides clear documentation, domain breakdowns, and filtering details. No custom tooling required. The scale means full downloads are large, but domain-specific subsets (e.g. AlgebraicStack only) are manageable.

### Complexity (7/10)
The arXiv mathematics subset reaches into research-frontier papers. The AlgebraicStack includes graduate-level Mathlib4 and AFP content alongside simpler material. Average complexity is high relative to human-authored competition datasets, though the corpus is intentionally broad rather than focused on hard problems.
