# Metamath (set.mm)

**Category:** Formal Libraries
**Link:** https://us.metamath.org/mpeuni/mmset.html

## Description

The core Metamath library (`set.mm`), containing ~40,000 formally verified proofs built from axiomatic set theory (ZFC) up through real analysis, number theory, topology, and abstract algebra. Metamath uses an unusually minimal and rigorous substitution-based proof checker — one of the strictest formalisms available — and has been developed continuously since the 1990s. The full library is a single self-contained file.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 7 |
| Level of Formalization | 10 |
| Ease of Use | 4 |
| Complexity | 6 |
| **Overall** | **6.6** |

## Justification

### Data Diversity (6/10)
Covers propositional and predicate logic, set theory, real and complex analysis, number theory, abstract algebra, and some topology. The foundation-up construction means the library includes many low-level logical lemmas not found in higher-level libraries. Coverage is broad but skewed toward foundational and classical results; modern research-frontier mathematics is thin.

### Size (7/10)
Approximately 40,000 proofs in `set.mm`, making it one of the older and larger formally verified corpora available. Growth is slower than Mathlib4 or AFP — the strict low-level formalism means each proof is labor-intensive to write.

### Level of Formalization (10/10)
Metamath's proof checker is arguably the most rigorous in the ecosystem. Proofs consist entirely of explicit substitution steps, with no automation or tactics; every logical step is mechanically verified. The formalism is so transparent that the checker itself is under 200 lines of C. Correctness is guaranteed at the deepest possible level.

### Ease of Use (4/10)
Metamath's notation and proof format are idiosyncratic and require dedicated tooling (the Metamath proof verifier, Metamath-lamp, or mmj2). Integration with modern ML pipelines is non-trivial; there is no equivalent of LeanDojo or PISA for Metamath. The single-file format is convenient for some purposes but awkward for structured extraction.

### Complexity (6/10)
The corpus spans from elementary logic to real analysis and number theory, but most theorems are classical results at the undergraduate-to-early-graduate level. The formalism is extremely verbose — simple results require many proof steps — which makes Metamath proofs harder to read than their mathematical content would suggest.
