# NaturalProofs

**Category:** Human-Authored Reference Datasets
**Link:** https://github.com/wellecks/naturalproofs)

## Description

Mathematical theorem statements and proofs scraped from ProofWiki and mathematics textbooks. Includes theorem statements, human-written proofs, and reference links. Designed for studying mathematical reasoning in natural language with access to a reference corpus.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 7 |
| Size | 6 |
| Level of Formalization | 2 |
| Ease of Use | 8 |
| Complexity | 6 |
| **Overall** | **5.8** |

## Justification

### Data Diversity (7/10)
ProofWiki covers a wide range of mathematical topics — number theory, analysis, algebra, topology, combinatorics — at varying levels of sophistication. The textbook component adds additional coverage. Good breadth for a natural language corpus.

### Size (6/10)
Tens of thousands of theorem-proof pairs. Substantial for a scraped mathematical corpus, though smaller than what could be extracted from the full arXiv or textbook digitization efforts.

### Level of Formalization (2/10)
Natural language proofs with no formal verification. ProofWiki proofs are human-written and often contain informal reasoning steps. Some may contain errors or gaps. The slight advantage over GSM8K or MATH is that ProofWiki proofs attempt genuine mathematical rigor, even if not machine-checkable.

### Ease of Use (8/10)
Well-documented with clean data formats. The reference retrieval aspect (linking theorems to their premises) is well-structured. Directly usable for training retrieval-augmented language models on informal mathematics.

### Complexity (6/10)
Spans elementary to upper-undergraduate mathematics. ProofWiki leans toward accessible, expository proofs rather than research-frontier results. More complex than competition problem collections on average, but below graduate-level research mathematics.
