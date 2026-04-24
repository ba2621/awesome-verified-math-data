# Coq Standard Library

**Category:** Formal Libraries
**Link:** https://coq.inria.fr/library/

## Description

The official standard library for the Coq proof assistant. Covers basic logic, arithmetic, sets, lists, strings, and core data structures. Ships with every Coq installation and forms the foundation for the Coq ecosystem.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 5 |
| Size | 5 |
| Level of Formalization | 10 |
| Ease of Use | 6 |
| Complexity | 5 |
| **Overall** | **6.2** |

## Justification

### Data Diversity (5/10)
Covers the essentials — natural numbers, integers, reals, sets, lists, booleans, strings — but does not aim for the breadth of Mathlib4 or AFP. More advanced Coq mathematics lives in community libraries (Mathematical Components, Coq-HoTT, etc.) rather than the standard library.

### Size (5/10)
Moderate in scale — thousands of definitions and lemmas, but small compared to Mathlib4 or AFP. The standard library is deliberately lean, delegating coverage to the community ecosystem.

### Level of Formalization (10/10)
Fully checked by the Coq kernel. The standard library is among the most trusted codebases in the formal methods world, having been in development and use for over three decades.

### Ease of Use (6/10)
Well-documented with searchable online reference. Coq has a mature toolchain (Proof General, CoqIDE, Rocq). However, Coq's tactic language is more complex than Lean 4's, and AI tooling for data extraction is less developed.

### Complexity (5/10)
The standard library deliberately stays at an accessible, foundational level. The mathematics covered is real analysis basics, integer arithmetic, and combinatorics — important but not deeply complex by research standards.
