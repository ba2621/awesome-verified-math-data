# awesome-verified-math-data
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

# awesome-verified-math-data [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of verified mathematical datasets — with a focus on formal, machine-checkable corpora for AI training and research.

---

## Why verified math data?

The bottleneck to AI progress in mathematics is not model architecture — it is data.

Most training data for math AI falls into the **human-authored** regime: textbooks, arXiv papers, Olympiad problems, and benchmarks like GSM8K or MATH. This data is valuable but bounded by what humans can produce and transcribe. It is also largely *unverified* — solutions may be wrong, proofs may be incomplete, and there is no formal guarantee of correctness.

**Verified (machine-checkable) mathematics** is different. Every proof has been checked by a formal proof assistant (e.g. Lean, Coq, Isabelle), meaning correctness is guaranteed by construction. This creates a fundamentally higher-quality training signal:

- **No hallucinated proofs.** The data is correct by definition.
- **Scalable.** Automated theorem provers can generate vast quantities of new, verified data beyond the human corpus.
- **Structured.** Formal libraries expose dependency graphs, lemma hierarchies, and tactic traces — metadata unavailable in natural language math.
- **Future-proof.** The frontier of AI math research is shifting toward formal reasoning; verified data is the substrate for that shift.

This repository aggregates existing verified math datasets, explains the landscape, and surfaces open research directions for the community.

---

## Contents

- [Formal Libraries](#formal-libraries)
- [Benchmarks & Evaluation Sets](#benchmarks--evaluation-sets)
- [Autoformalization Datasets](#autoformalization-datasets)
- [Synthetic & Generated Corpora](#synthetic--generated-corpora)
- [Human-Authored Reference Datasets](#human-authored-reference-datasets)
- [Tools & Infrastructure](#tools--infrastructure)
- [Research Directions & Open Problems](#research-directions--open-problems)
- [Contributing](#contributing)

---

## Formal Libraries

The foundational corpora of machine-verified mathematics.

- **[Mathlib4](https://github.com/leanprover-community/mathlib4)** — The canonical community mathematics library for Lean 4. Covers algebra, analysis, topology, number theory, and more. The de facto standard corpus for formal math AI research.
- **[Lean 4 Core](https://github.com/leanprover/lean4)** — Core Lean 4 library, including foundational logic and type theory.
- **[Archive of Formal Proofs (AFP)](https://www.isa-afp.org/)** — A large collection of formal proofs in Isabelle/HOL, spanning thousands of entries across many mathematical domains.
- **[Coq Standard Library](https://coq.inria.fr/library/)** — The standard library for the Coq proof assistant.
- **[UniMath](https://github.com/UniMath/UniMath)** — A library of mathematics formalized in Coq using the univalent foundations perspective.
- **[HOL Light](https://www.cl.cam.ac.uk/~jrh13/hol-light/)** — A proof assistant and its accompanying library, notably including a formal proof of the Kepler conjecture.

---

## Benchmarks & Evaluation Sets

Curated problem sets for evaluating formal and informal math reasoning.

- **[MiniF2F](https://github.com/openai/miniF2F)** — 488 competition-level math problems formalized in Lean, Isabelle, HOL Light, and Metamath. The standard benchmark for formal theorem proving.
- **[ProofNet](https://github.com/zhangir-azerbayev/ProofNet)** — Undergraduate-level mathematical theorems with formal Lean 4 statements, designed to evaluate autoformalization.
- **[FIMO](https://arxiv.org/abs/2309.04295)** — IMO problems formalized in Lean 4.
- **[LeanDojo Benchmark](https://leandojo.org/)** — Theorems and proofs extracted from Mathlib4, with tactic-level annotations for training and evaluation of proof search models.

---

## Autoformalization Datasets

Datasets pairing informal (natural language) mathematics with formal statements or proofs.

- **[MATH-to-Lean](https://github.com/wellecks/ntptutorial)** — Datasets and tools from research on neural theorem proving, including informal-formal pairs.
- **[AutoFormalization with LLMs (He et al.)](https://arxiv.org/abs/2205.12615)** — Dataset from early work on using language models to translate informal math to Lean.
- **[MMA (Multilingual Mathematical Autoformalization)](https://arxiv.org/abs/2311.02155)** — Informal-formal pairs across multiple languages and proof assistants.

---

## Synthetic & Generated Corpora

Machine-generated datasets for scaling beyond the human-authored corpus.

- **[LEGO-Prover](https://arxiv.org/abs/2310.00656)** — Grows a library of verified Lean lemmas via iterative generation, creating an expanding corpus of machine-verified skills.
- **[Hypertree Proof Search Data](https://arxiv.org/abs/2205.11491)** — Proof search traces from Expert Iteration over formal libraries.
- **[Draft-Sketch-Prove](https://arxiv.org/abs/2210.12283)** — Generated proof attempts with formal verification in the loop.

---

## Human-Authored Reference Datasets

Informal datasets included for context and cross-referencing. These are valuable for pretraining and autoformalization but are not formally verified.

- **[MATH](https://github.com/hendrycks/math)** — 12,500 competition math problems with step-by-step solutions, across 7 subjects.
- **[GSM8K](https://github.com/openai/grade-school-math)** — 8,500 grade-school math word problems from OpenAI.
- **[NaturalProofs](https://github.com/wellecks/naturalproofs)** — Mathematical theorem statements and proofs scraped from ProofWiki and textbooks.
- **[AMPS](https://github.com/hendrycks/math)** — Khan Academy and Mathematica problem sets used in MATH pretraining.
- **[Lean Workbook](https://arxiv.org/abs/2406.03847)** — ~57k informal math problems with Lean 4 statements (partially verified).

---

## Tools & Infrastructure

Software for working with formal math data.

- **[LeanDojo](https://github.com/lean-dojo/LeanDojo)** — Toolkit for extracting data from Lean repositories and interacting with Lean programmatically. Essential for dataset construction.
- **[Pantograph](https://github.com/lenianiva/Pantograph)** — A Lean 4 REPL for machine-to-machine theorem proving interaction.
- **[PyPantograph](https://github.com/lenianiva/PyPantograph)** — Python bindings for Pantograph.
- **[mathlib4-data-extraction](https://github.com/leanprover-community/mathlib4)** — Scripts and utilities for extracting structured data from Mathlib4.
- **[REPL (Lean 4)](https://github.com/leanprover-community/repl)** — An official Lean 4 REPL for programmatic proof interaction.

---

## Research Directions & Open Problems

Key gaps and open questions in the verified math data ecosystem.

- **Coverage gaps.** Mathlib4 is deep in pure mathematics but thin in areas like combinatorics, probability, and applied math. These domains are underrepresented relative to their importance.
- **Tactic-level datasets.** Most datasets capture theorem statements and final proofs, but intermediate tactic traces (the step-by-step proof state) are harder to extract at scale and are underutilized.
- **Autoformalization at scale.** Translating the existing corpus of arXiv mathematics into verified Lean statements remains unsolved. High-quality informal-formal paired datasets are scarce.
- **Proof diversity.** Libraries tend to contain one proof per theorem. Datasets with multiple, stylistically diverse proofs of the same statement would better support learning generalization.
- **Cross-assistant alignment.** MiniF2F is the only major benchmark formalized across multiple proof assistants. Broader cross-system datasets would help compare systems and enable transfer.
- **Dynamic / evolving benchmarks.** Most benchmarks are static. A living benchmark that adds new problems as they are formalized (e.g. from recent competition seasons) is an open infrastructure challenge.

---

## Contributing

Contributions are welcome and encouraged. Please read the [contribution guidelines](CONTRIBUTING.md) before submitting a pull request.

To add a dataset, tool, or research direction:
1. Check that it fits one of the existing categories (or propose a new one).
2. For verified datasets, confirm the data is formally checked by a proof assistant.
3. Provide a brief, accurate description and a working link.
4. Submit a pull request.

---

## License

[CC0 1.0 Universal](LICENSE) — this list is public domain.
