# Lean 4 Core

**Category:** Formal Libraries
**Link:** https://github.com/leanprover/lean4

## Description

The core Lean 4 library, including foundational logic, type theory, basic data structures, and the standard prelude. Maintained by the Lean development team at Microsoft Research and Amazon.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 4 |
| Size | 4 |
| Level of Formalization | 10 |
| Ease of Use | 6 |
| Complexity | 5 |
| **Overall** | **5.8** |

## Justification

### Data Diversity (4/10)
Deliberately narrow in scope — foundational logic, inductive types, basic list and number operations, and core tactics. Not intended to cover broad mathematical content; that role belongs to Mathlib4.

### Size (4/10)
Much smaller than Mathlib4. The core library contains thousands of definitions and lemmas but is not a large-scale mathematical corpus by itself.

### Level of Formalization (10/10)
Fully verified by the Lean 4 kernel. The core library is the most trusted layer of the ecosystem.

### Ease of Use (6/10)
Well-documented as a reference for Lean itself. However, the content is oriented toward programming language foundations rather than mathematical applications, making it less immediately useful for math AI research without augmentation from Mathlib4.

### Complexity (5/10)
The mathematics is foundational rather than complex — propositions about natural numbers, lists, and basic logic. The type-theoretic content can be subtle, but the mathematical depth is limited compared to Mathlib4 or AFP.
