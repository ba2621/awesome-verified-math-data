# LEGO-Prover

**Category:** Autoformalization Datasets / Synthetic & Generated Corpora
**Link:** https://arxiv.org/abs/2310.00656

## Description

A system and corpus that grows a library of verified Lean lemmas through iterative generation. An LLM proposes new lemmas, attempts to prove them in Lean, and those that verify are added to the growing skill library. The corpus expands continuously as new lemmas are proved.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 6 |
| Level of Formalization | 9 |
| Ease of Use | 6 |
| Complexity | 6 |
| **Overall** | **6.6** |

## Justification

### Data Diversity (6/10)
The iterative generation process explores a reasonably broad space of lemmas, but the distribution is shaped by what LLMs choose to generate, which skews toward tractable, common patterns rather than uniformly covering all of mathematics.

### Size (6/10)
Grows over iterations; reported size depends on the version and run configuration. Moderate scale — larger than a curated benchmark but smaller than Mathlib4. The self-expanding nature means size is not fixed.

### Level of Formalization (9/10)
Only lemmas that have been verified by the Lean kernel are added to the library. This is a strong formalization guarantee: the corpus is correct by construction, even though it is machine-generated rather than human-authored.

### Ease of Use (6/10)
The system is described in the paper and code is available, but running the generation pipeline requires a working Lean 4 setup and compute resources. The resulting corpus is usable but requires some effort to extract.

### Complexity (6/10)
The generated lemmas tend to be useful helper lemmas and intermediate results rather than deep theorems. Complexity is moderate — the system is designed to build up reusable skills, not to prove the hardest open problems.
