# TopoAlign Python

**Category:** Autoformalization Datasets
**Link:** https://huggingface.co/datasets/Formal-Math-Reasoning/TopoAlign_Python

## Description

A large-scale dataset of ~250k Python code examples paired with dependencies and docstrings, intended for formal mathematical reasoning tasks. Each entry is a dependency–docstring–implementation triplet extracted from real Python codebases. Unlike proof-assistant datasets, the "formal" language here is Python rather than Lean or Coq — the dataset targets code generation and retrieval tasks over mathematical software rather than formal proof synthesis.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 9 |
| Level of Formalization | 2 |
| Ease of Use | 7 |
| Complexity | 3 |
| **Overall** | **5.4** |

## Justification

### Data Diversity (6/10)
Covers diverse Python code contexts including mathematical modeling, ML implementations, and API interactions. Breadth is real, but it is not mathematical diversity in the proof-theoretic sense — there are no domain labels for algebra, topology, or number theory. Most entries are general-purpose code rather than mathematics-specific implementations.

### Size (9/10)
~250,000 examples is very large, second only to Big-Math-RL-Verified in this list. Scale is the primary strength of this dataset for pretraining or retrieval model training.

### Level of Formalization (2/10)
Python is not a formal proof assistant. There is no kernel-level guarantee of mathematical correctness — code may run or compile but contain mathematical errors. This is a hard ceiling: however well-structured the data is, it lacks the formal verification guarantee that distinguishes proof-assistant corpora.

### Ease of Use (7/10)
Hosted on HuggingFace in parquet format with a clear three-column schema (dependency, docstring, main). CC-BY-4.0 license. No special tooling required. The large column widths (up to 854k characters for dependencies) require attention when loading into memory-constrained environments.

### Complexity (3/10)
The underlying code complexity is moderate Python engineering, not graduate mathematics. Docstrings describe function behavior rather than mathematical theorems. Useful for code LLMs with a math focus but not for training formal theorem provers.
