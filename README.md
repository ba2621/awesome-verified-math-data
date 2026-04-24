
# awesome-verified-math-data [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of verified mathematical datasets — with a focus on formal, machine-checkable corpora for AI training and research.

---

**28 datasets · ~6.8 million total datapoints · ~800k+ formally verified theorems and proofs**

The formally verified subset alone — drawn from Mathlib4, AFP, the Coq libraries, LeanDojo, lean-mathlib-rag, and related corpora — exceeds the data threshold typically required to fine-tune a 1–7B parameter math-focused language model (which is on the order of tens of thousands to a few hundred thousand high-quality examples). The full corpus, extending to competition problems, autoformalization pairs, RL-verified problems, and informal reference datasets, provides sufficient scale for continued pretraining or domain-adaptive pretraining of a small specialized model.

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

For each dataset, I have created an "empirical" evaluation based on a few factors of when I inspect the datasets. On a scale from 1-10, each dataset is ranked on:
- Data diversity
- Size
- Level of formalization
- Ease of use
- Complexity (more complex datasets and "tougher" problems are ranked higher)

The evaluation of the dataset is then a simple average of these five factors. Full evaluations with per-factor justifications are in the [`evaluations/`](evaluations/) folder — see the [index](evaluations/index.md) for a ranked overview of all datasets.

---

## Contents

- [Formal Libraries](#formal-libraries)
- [Benchmarks & Evaluation Sets](#benchmarks--evaluation-sets)
- [Autoformalization Datasets](#autoformalization-datasets)
- [Synthetic & Generated Corpora](#synthetic--generated-corpora)
- [Human-Authored Reference Datasets](#human-authored-reference-datasets)
- [Tools & Infrastructure](#tools--infrastructure)
- [Research Directions & Open Problems](#research-directions--open-problems)
- [Dataset Evaluations](evaluations/index.md)
- [System Prompts](#system-prompts)
- [Contributing](#contributing)

---

## Formal Libraries

The foundational corpora of machine-verified mathematics.

- **[Mathlib4](https://github.com/leanprover-community/mathlib4)** — The canonical community mathematics library for Lean 4. Covers algebra, analysis, topology, number theory, and more. The de facto standard corpus for formal math AI research. | [Evaluation](evaluations/formal-libraries/mathlib4.md) — **8.6/10**
- **[Lean 4 Core](https://github.com/leanprover/lean4)** — Core Lean 4 library, including foundational logic and type theory. | [Evaluation](evaluations/formal-libraries/lean4-core.md) — **5.8/10**
- **[Archive of Formal Proofs (AFP)](https://www.isa-afp.org/)** — A large collection of formal proofs in Isabelle/HOL, spanning thousands of entries across many mathematical domains. | [Evaluation](evaluations/formal-libraries/afp.md) — **8.2/10**
- **[Coq Standard Library](https://coq.inria.fr/library/)** — The standard library for the Coq proof assistant. | [Evaluation](evaluations/formal-libraries/coq-standard-library.md) — **6.2/10**
- **[UniMath](https://github.com/UniMath/UniMath)** — A library of mathematics formalized in Coq using the univalent foundations perspective. | [Evaluation](evaluations/formal-libraries/unimath.md) — **6.2/10**
- **[HOL Light](https://www.cl.cam.ac.uk/~jrh13/hol-light/)** — A proof assistant and its accompanying library, notably including a formal proof of the Kepler conjecture. | [Evaluation](evaluations/formal-libraries/hol-light.md) — **6.8/10**
- **[Coq-MathComp](https://huggingface.co/datasets/phanerozoic/Coq-MathComp)** — ~20k structured entries extracted from the Mathematical Components (MathComp) Coq library, covering algebra, finite group theory, and field theory using SSReflect. | [Evaluation](evaluations/formal-libraries/coq-mathcomp.md) — **6.8/10**

---

## Benchmarks & Evaluation Sets

Curated problem sets for evaluating formal and informal math reasoning.

- **[MiniF2F](https://github.com/openai/miniF2F)** — 488 competition-level math problems formalized in Lean, Isabelle, HOL Light, and Metamath. The standard benchmark for formal theorem proving. | [Evaluation](evaluations/benchmarks/minif2f.md) — **7.0/10**
- **[ProofNet](https://github.com/zhangir-azerbayev/ProofNet)** — Undergraduate-level mathematical theorems with formal Lean 4 statements, designed to evaluate autoformalization. | [Evaluation](evaluations/benchmarks/proofnet.md) — **6.0/10**
- **[FIMO](https://arxiv.org/abs/2309.04295)** — IMO problems formalized in Lean 4. | [Evaluation](evaluations/benchmarks/fimo.md) — **6.2/10**
- **[LeanDojo Benchmark](https://leandojo.org/)** — Theorems and proofs extracted from Mathlib4, with tactic-level annotations for training and evaluation of proof search models. | [Evaluation](evaluations/benchmarks/leandojo-benchmark.md) — **8.4/10**
- **[Lean Math Formal Corpus](https://huggingface.co/datasets/iiis-lean/lean-math-formal-corpus)** — 2,880 compile-validated Lean 4 proofs of IMO, APMO, and EGMO olympiad problems, with paired natural language and formal representations and repair-tracking metadata. | [Evaluation](evaluations/benchmarks/lean-math-formal-corpus.md) — **6.8/10**
- **[mathematic-coq](https://huggingface.co/datasets/Pawitt/mathematic-coq)** — 6,207 Coq proof examples from the Mathematical Components library in context–claim–proof format, spanning analysis, number theory, and algebra. | [Evaluation](evaluations/benchmarks/mathematic-coq.md) — **5.4/10**

---

## Autoformalization Datasets

Datasets pairing informal (natural language) mathematics with formal statements or proofs.

- **[MATH-to-Lean](https://github.com/wellecks/ntptutorial)** — Datasets and tools from research on neural theorem proving, including informal-formal pairs. | [Evaluation](evaluations/autoformalization/math-to-lean.md) — **6.2/10**
- **[AutoFormalization with LLMs (He et al.)](https://arxiv.org/abs/2205.12615)** — Dataset from early work on using language models to translate informal math to Lean. | [Evaluation](evaluations/autoformalization/autoformalization-he-et-al.md) — **5.4/10**
- **[MMA (Multilingual Mathematical Autoformalization)](https://arxiv.org/abs/2311.02155)** — Informal-formal pairs across multiple languages and proof assistants. | [Evaluation](evaluations/autoformalization/mma.md) — **6.8/10**
- **[FormalMATH-All](https://huggingface.co/datasets/SphereLab/FormalMATH-All)** — 5,560 competition math problems (AMC, AIME, Chinese competitions) autoformalized into Lean 4, with compiler validation feedback and bilingual (EN/ZH) coverage across 802 mathematical subdomains. | [Evaluation](evaluations/autoformalization/formalmath-all.md) — **7.0/10**
- **[TopoAlign Python](https://huggingface.co/datasets/Formal-Math-Reasoning/TopoAlign_Python)** — ~250k Python code examples paired with dependencies and docstrings for formal mathematical reasoning tasks. Note: uses Python as the formal language rather than a proof assistant. | [Evaluation](evaluations/autoformalization/topoalign-python.md) — **5.4/10**

---

## Synthetic & Generated Corpora

Machine-generated datasets for scaling beyond the human-authored corpus.

- **[LEGO-Prover](https://arxiv.org/abs/2310.00656)** — Grows a library of verified Lean lemmas via iterative generation, creating an expanding corpus of machine-verified skills. | [Evaluation](evaluations/autoformalization/lego-prover.md) — **6.6/10**
- **[Hypertree Proof Search Data](https://arxiv.org/abs/2205.11491)** — Proof search traces from Expert Iteration over formal libraries. | [Evaluation](evaluations/synthetic/hypertree-proof-search.md) — **6.6/10**
- **[Draft-Sketch-Prove](https://arxiv.org/abs/2210.12283)** — Generated proof attempts with formal verification in the loop. | [Evaluation](evaluations/synthetic/draft-sketch-prove.md) — **6.0/10**
- **[Big-Math-RL-Verified](https://huggingface.co/datasets/SynthLabsAI/Big-Math-RL-Verified)** — Largest open-source dataset of high-quality mathematical problems, curated specifically for reinforcement learning (RL) training in language models. 250k rigorously filtered and verified problems. | [Evaluation](evaluations/synthetic/big-math-rl-verified.md) — **8.0/10**
- **[lean-mathlib-rag](https://huggingface.co/datasets/pkuAI4M/lean_mathlib_rag)** — 92k tactic-state pairs extracted from Mathlib for retrieval-augmented generation (RAG) theorem proving, with tactic annotations and proof states. | [Evaluation](evaluations/synthetic/lean-mathlib-rag.md) — **7.6/10**

---

## Human-Authored Reference Datasets

Informal datasets included for context and cross-referencing. These are valuable for pretraining and autoformalization but are not formally verified.

- **[MATH](https://github.com/hendrycks/math)** — 12,500 competition math problems with step-by-step solutions, across 7 subjects. | [Evaluation](evaluations/human-authored/math.md) — **6.0/10**
- **[GSM8K](https://github.com/openai/grade-school-math)** — 8,500 grade-school math word problems from OpenAI. | [Evaluation](evaluations/human-authored/gsm8k.md) — **4.2/10**
- **[NaturalProofs](https://github.com/wellecks/naturalproofs)** — Mathematical theorem statements and proofs scraped from ProofWiki and textbooks. | [Evaluation](evaluations/human-authored/naturalproofs.md) — **5.8/10**
- **[AMPS](https://github.com/hendrycks/math)** — Khan Academy and Mathematica problem sets used in MATH pretraining. | [Evaluation](evaluations/human-authored/amps.md) — **5.6/10**
- **[Lean Workbook](https://arxiv.org/abs/2406.03847)** — ~57k informal math problems with Lean 4 statements (partially verified). | [Evaluation](evaluations/human-authored/lean-workbook.md) — **6.4/10**

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

- **Tactic-level datasets.** Most datasets capture theorem statements and final proofs, but intermediate tactic traces (the step-by-step proof state) are harder to extract at scale and are underutilized.
- **Autoformalization at scale.** Translating the existing corpus of arXiv mathematics into verified Lean statements remains unsolved. High-quality informal-formal paired datasets are scarce.
- **Proof diversity.** Libraries tend to contain one proof per theorem. Datasets with multiple, stylistically diverse proofs of the same statement would better support learning generalization.
- **Automation** How can we automate the creation of formal verified math data?

---

## System Prompts

Persona-based system prompts for interacting with an LLM about this repository and its datasets. Each prompt is tailored to a different background and set of goals, so the assistant can give appropriately targeted responses rather than generic ones.

| Persona | Description |
|---------|-------------|
| [AI Researcher / Model Developer](system-prompts/ai-researcher-model-developer.md) | ML practitioner evaluating datasets for training or benchmarking neural theorem provers and reasoning models |
| [PhD Mathematics Student](system-prompts/phd-math-student.md) | Graduate student learning to use formal verification tools and datasets for research |
| [Undergraduate Mathematics Student](system-prompts/undergraduate-student.md) | Undergrad getting started with formal math and proof assistants |
| [Middle School Math Prodigy](system-prompts/middle-school-math-prodigy.md) | Competition math student (AMC/AIME/MATHCOUNTS) exploring formal mathematics for the first time |
| [Software Engineer Curious About AI and Math](system-prompts/software-engineer-ai-math-curious.md) | Engineer with a software background exploring the intersection of LLMs and formal mathematics |
| [Terence Tao](system-prompts/terence-tao.md) | Research mathematician at the frontier, exploring formal verification as a tool for research |

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
