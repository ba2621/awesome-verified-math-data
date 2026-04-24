# HOL Light

**Category:** Formal Libraries
**Link:** https://www.cl.cam.ac.uk/~jrh13/hol-light/

## Description

A lightweight proof assistant in the HOL family, implemented in OCaml. Notable for containing a formal proof of the Kepler conjecture (the Flyspeck project) and Harrison's formalization of complex analysis and number theory. Prioritizes a minimal, highly trusted logical kernel.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 6 |
| Level of Formalization | 10 |
| Ease of Use | 4 |
| Complexity | 8 |
| **Overall** | **6.8** |

## Justification

### Data Diversity (6/10)
Has notable depth in real and complex analysis, number theory, and geometry (including the full Flyspeck proof of the Kepler conjecture). Diversity is moderate — the library reflects the research interests of its primary contributors rather than a community-driven breadth effort.

### Size (6/10)
Moderate size. Smaller than Mathlib4 or AFP in total theorem count, but contains several landmark results unavailable elsewhere in formal form.

### Level of Formalization (10/10)
Among the most trusted formal systems in existence. HOL Light's kernel is extremely small and has been independently audited. The Flyspeck proof (>20 years of work) provides a gold standard for formal verification at scale.

### Ease of Use (4/10)
OCaml-based and lacks modern IDE integrations or interactive tactic browsers. Less popular in the current AI research community than Lean 4. Extracting structured data requires significant custom tooling. Documentation is primarily academic papers rather than onboarding guides.

### Complexity (8/10)
Contains some of the most complex results in any formal library — the Kepler conjecture proof, deep results in complex analysis, and serious number theory. The average complexity of the library is high relative to its size.
