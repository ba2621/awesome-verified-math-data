# UniMath

**Category:** Formal Libraries
**Link:** https://github.com/UniMath/UniMath

## Description

A library of mathematics formalized in Coq using the univalent foundations (HoTT) perspective, initiated by Vladimir Voevodsky. Emphasizes foundational correctness using the univalence axiom and covers category theory, algebra, and type-theoretic constructions.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 5 |
| Size | 4 |
| Level of Formalization | 10 |
| Ease of Use | 4 |
| Complexity | 8 |
| **Overall** | **6.2** |

## Justification

### Data Diversity (5/10)
Focused on a specific foundational perspective (univalent foundations / HoTT) rather than broad mathematical coverage. Covers category theory, algebra, and combinatorics but does not attempt the breadth of Mathlib4 or AFP.

### Size (4/10)
Substantially smaller than the major libraries. Active but niche community; the scope is intentionally constrained to mathematics compatible with the univalent foundations program.

### Level of Formalization (10/10)
Fully verified in Coq. The univalent foundations approach actually strengthens the formalization: concepts like isomorphism and equality are handled more carefully than in classical foundations, making the proofs more structurally meaningful.

### Ease of Use (4/10)
Requires understanding of homotopy type theory to work with effectively. The conceptual overhead is high even for experts in other proof assistants. AI tooling is minimal; data extraction is non-trivial.

### Complexity (8/10)
The mathematics is genuinely complex — category theory, topos theory, and constructions from algebraic topology formalized under a demanding foundational framework. The combination of advanced mathematics and a non-standard foundation makes this one of the more intellectually demanding corpora.
