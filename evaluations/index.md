# Dataset Evaluations

Empirical evaluations of all datasets in awesome-verified-math-data, scored 1–10 on five factors:

- **Data Diversity** — breadth of mathematical domains, proof styles, or problem types covered
- **Size** — number of theorems, problems, or proof traces
- **Level of Formalization** — degree to which the data is formally machine-checked (10 = fully verified)
- **Ease of Use** — quality of tooling, documentation, and accessibility for AI research
- **Complexity** — difficulty of the underlying mathematics or problems

The overall score is the simple average of the five factors.

---

## Formal Libraries

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [Mathlib4](formal-libraries/mathlib4.md) | 9 | 9 | 10 | 7 | 8 | **8.6** |
| [Archive of Formal Proofs](formal-libraries/afp.md) | 9 | 9 | 10 | 6 | 7 | **8.2** |
| [HOL Light](formal-libraries/hol-light.md) | 6 | 6 | 10 | 4 | 8 | **6.8** |
| [Coq-MathComp](formal-libraries/coq-mathcomp.md) | 6 | 6 | 10 | 5 | 7 | **6.8** |
| [Metamath](formal-libraries/metamath.md) | 6 | 7 | 10 | 4 | 6 | **6.6** |
| [Coq Standard Library](formal-libraries/coq-standard-library.md) | 5 | 5 | 10 | 6 | 5 | **6.2** |
| [UniMath](formal-libraries/unimath.md) | 5 | 4 | 10 | 4 | 8 | **6.2** |
| [Lean 4 Core](formal-libraries/lean4-core.md) | 4 | 4 | 10 | 6 | 5 | **5.8** |

## Benchmarks & Evaluation Sets

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [LeanDojo Benchmark](benchmarks/leandojo-benchmark.md) | 8 | 8 | 10 | 9 | 7 | **8.4** |
| [ISARSTEP](benchmarks/isarstep.md) | 6 | 8 | 10 | 5 | 7 | **7.2** |
| [MiniF2F](benchmarks/minif2f.md) | 6 | 3 | 9 | 9 | 8 | **7.0** |
| [Lean Math Formal Corpus](benchmarks/lean-math-formal-corpus.md) | 5 | 3 | 10 | 7 | 9 | **6.8** |
| [PutnamBench](benchmarks/putnam-bench.md) | 5 | 3 | 9 | 7 | 10 | **6.8** |
| [FIMO](benchmarks/fimo.md) | 3 | 2 | 9 | 7 | 10 | **6.2** |
| [ProofNet](benchmarks/proofnet.md) | 5 | 3 | 8 | 8 | 6 | **6.0** |
| [mathematic-coq](benchmarks/mathematic-coq.md) | 4 | 4 | 9 | 4 | 6 | **5.4** |

## Autoformalization Datasets

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [MMA](autoformalization/mma.md) | 8 | 6 | 7 | 7 | 6 | **6.8** |
| [LEGO-Prover](autoformalization/lego-prover.md) | 6 | 6 | 9 | 6 | 6 | **6.6** |
| [FormalMATH-All](autoformalization/formalmath-all.md) | 7 | 5 | 8 | 7 | 8 | **7.0** |
| [MATH-to-Lean](autoformalization/math-to-lean.md) | 6 | 5 | 7 | 7 | 6 | **6.2** |
| [AutoFormalization (He et al.)](autoformalization/autoformalization-he-et-al.md) | 5 | 4 | 7 | 6 | 5 | **5.4** |
| [TopoAlign Python](autoformalization/topoalign-python.md) | 6 | 9 | 2 | 7 | 3 | **5.4** |

## Synthetic & Generated Corpora

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [Big-Math-RL-Verified](synthetic/big-math-rl-verified.md) | 8 | 10 | 7 | 8 | 7 | **8.0** |
| [lean-mathlib-rag](synthetic/lean-mathlib-rag.md) | 8 | 8 | 10 | 5 | 7 | **7.6** |
| [Hypertree Proof Search Data](synthetic/hypertree-proof-search.md) | 7 | 6 | 8 | 5 | 7 | **6.6** |
| [Draft-Sketch-Prove](synthetic/draft-sketch-prove.md) | 6 | 5 | 7 | 6 | 6 | **6.0** |

## Human-Authored Reference Datasets

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [Proof Pile II / AlgebraicStack](human-authored/proof-pile-ii.md) | 9 | 10 | 3 | 8 | 7 | **7.4** |
| [NuminaMath-CoT](human-authored/numina-math-cot.md) | 8 | 10 | 1 | 9 | 7 | **7.0** |
| [Lean Workbook](human-authored/lean-workbook.md) | 7 | 7 | 5 | 7 | 6 | **6.4** |
| [MATH](human-authored/math.md) | 7 | 6 | 1 | 9 | 7 | **6.0** |
| [NaturalProofs](human-authored/naturalproofs.md) | 7 | 6 | 2 | 8 | 6 | **5.8** |
| [AMPS](human-authored/amps.md) | 6 | 8 | 1 | 8 | 5 | **5.6** |
| [GSM8K](human-authored/gsm8k.md) | 3 | 5 | 1 | 10 | 2 | **4.2** |

---

## Overall Rankings

| Rank | Dataset | Overall Score |
|------|---------|--------------|
| 1 | Mathlib4 | 8.6 |
| 2 | LeanDojo Benchmark | 8.4 |
| 3 | Archive of Formal Proofs | 8.2 |
| 4 | Big-Math-RL-Verified | 8.0 |
| 5 | lean-mathlib-rag | 7.6 |
| 6 | Proof Pile II / AlgebraicStack | 7.4 |
| 7 | ISARSTEP | 7.2 |
| 8 | MiniF2F | 7.0 |
| 9 | FormalMATH-All | 7.0 |
| 10 | NuminaMath-CoT | 7.0 |
| 11 | HOL Light | 6.8 |
| 12 | MMA | 6.8 |
| 13 | Coq-MathComp | 6.8 |
| 14 | Lean Math Formal Corpus | 6.8 |
| 15 | PutnamBench | 6.8 |
| 16 | LEGO-Prover | 6.6 |
| 17 | Hypertree Proof Search Data | 6.6 |
| 18 | Metamath | 6.6 |
| 19 | Lean Workbook | 6.4 |
| 20 | Coq Standard Library | 6.2 |
| 21 | UniMath | 6.2 |
| 22 | FIMO | 6.2 |
| 23 | MATH-to-Lean | 6.2 |
| 24 | MATH | 6.0 |
| 25 | ProofNet | 6.0 |
| 26 | Draft-Sketch-Prove | 6.0 |
| 27 | Lean 4 Core | 5.8 |
| 28 | NaturalProofs | 5.8 |
| 29 | AMPS | 5.6 |
| 30 | AutoFormalization (He et al.) | 5.4 |
| 31 | TopoAlign Python | 5.4 |
| 32 | mathematic-coq | 5.4 |
| 33 | GSM8K | 4.2 |
