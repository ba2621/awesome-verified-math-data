# lean-mathlib-rag

**Category:** Synthetic & Generated Corpora
**Link:** https://huggingface.co/datasets/pkuAI4M/lean_mathlib_rag

## Description

A retrieval-augmented generation (RAG) dataset of 92,152 tactic-state pairs extracted from Lean's Mathlib library by Peking University's AI4M group. Each entry captures a proof state, the tactic applied to advance that state, a commented version of the tactic, and an input representation. Designed to support tactic prediction and retrieval-based theorem proving in Lean.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 8 |
| Size | 8 |
| Level of Formalization | 10 |
| Ease of Use | 5 |
| Complexity | 7 |
| **Overall** | **7.6** |

## Justification

### Data Diversity (8/10)
Inherits Mathlib's comprehensive coverage: algebra, analysis, topology, number theory, combinatorics, category theory, and more. Tactic-state pairs span the full breadth of the library, capturing diverse proof strategies rather than a narrow subdomain.

### Size (8/10)
92,152 entries is substantial — in the same order of magnitude as LeanDojo Benchmark and among the larger tactic-level datasets available. Enough data to train meaningful retrieval or tactic prediction models.

### Level of Formalization (10/10)
All proof states and tactics are extracted from successfully compiled Mathlib proofs. Every tactic in the dataset was accepted by the Lean 4 kernel — there are no approximations or unverified entries.

### Ease of Use (5/10)
The README is sparse and the dataset access requires users to agree to share their contact information with the authors (pkuAI4M). No example notebooks or documentation on field semantics are provided. The data format (parquet, five columns) is clean once accessed, but the onboarding friction is notable.

### Complexity (7/10)
Mathlib-level mathematics — predominantly graduate and research-level content across many fields. Tactic-level granularity captures step-by-step proof difficulty rather than just the final result, which raises practical utility for proof search but the per-tactic complexity varies widely.
