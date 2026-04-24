# Coq-MathComp

**Category:** Formal Libraries
**Link:** https://huggingface.co/datasets/phanerozoic/Coq-MathComp

## Description

A structured dataset of ~20k entries extracted from the Mathematical Components (MathComp) library for Coq, covering formalized algebra, finite group theory, character theory, and field theory using the SSReflect proof language and Hierarchy Builder. Each entry captures a declaration (lemma, definition, structure) with its type, imports, source filename, and symbolic name. MathComp is the library underlying the formalized proof of the Feit-Thompson theorem and is a canonical source of advanced algebraic mathematics in Coq.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 6 |
| Level of Formalization | 10 |
| Ease of Use | 5 |
| Complexity | 7 |
| **Overall** | **6.8** |

## Justification

### Data Diversity (6/10)
Strong coverage of algebra, finite group theory, solvable groups, character theory, order theory, and field theory — the areas in which MathComp specializes. Less coverage of analysis, topology, or number theory relative to Mathlib or AFP. Algebra-heavy by design rather than omission.

### Size (6/10)
19,924 entries across 98 source files is a meaningful dataset. Smaller than AFP or Mathlib but larger than most competition-focused corpora. The 19 declaration types (lemma, definition, HB.structure, etc.) add useful structural variety.

### Level of Formalization (10/10)
Extracted directly from the formally verified MathComp library, which has been machine-checked by Coq's kernel. Every entry represents a theorem or definition that has been verified. MathComp's SSReflect style enforces a particularly disciplined proof discipline.

### Ease of Use (5/10)
SSReflect proof syntax is idiomatic and significantly different from standard Coq or Lean. The `docstring` field is empty in current data. CeCILL-B license is permissive but less familiar than MIT/CC. Limited downloads (21) suggest the community has not yet built significant tooling around this specific extract.

### Complexity (7/10)
MathComp formalizes advanced algebra including finite group theory (the Feit-Thompson theorem required MathComp). The mathematics is genuinely difficult graduate-to-research level, though the individual lemmas vary widely in complexity.
