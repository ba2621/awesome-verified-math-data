# Archive of Formal Proofs (AFP)

**Category:** Formal Libraries
**Link:** https://www.isa-afp.org/

## Description

A large, peer-reviewed collection of formal proofs in Isabelle/HOL. Organized as a journal-style archive with thousands of individual entries, each covering a distinct mathematical result or algorithm. Spans number theory, algebra, combinatorics, complexity theory, and more.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 9 |
| Size | 9 |
| Level of Formalization | 10 |
| Ease of Use | 6 |
| Complexity | 7 |
| **Overall** | **8.2** |

## Justification

### Data Diversity (9/10)
Over 800 entries covering an enormous range of mathematical and computer science topics — number theory, group theory, graph theory, cryptographic protocols, automata, game theory, and more. Arguably more thematically diverse than Mathlib4, though with less coherence as a unified library.

### Size (9/10)
Hundreds of thousands of theorems spread across thousands of files. One of the largest formally verified corpora in existence, comparable in scale to Mathlib4.

### Level of Formalization (10/10)
Every entry is fully checked by the Isabelle/HOL proof assistant. Entries undergo peer review before inclusion, giving an additional quality layer beyond mere mechanical checking.

### Ease of Use (6/10)
Isabelle/HOL is a mature but less trendy system than Lean 4, and AI tooling for it is less developed. Extracting structured data (tactic traces, premise sets) is harder than with LeanDojo. The entry format is relatively self-contained, which helps.

### Complexity (7/10)
Ranges from elementary to graduate-level. Some entries prove highly non-trivial results (e.g. primality of large numbers, combinatorial identities, verified compilers), but many are expository or cover well-known results at moderate difficulty.
