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
| [Coq Standard Library](formal-libraries/coq-standard-library.md) | 5 | 5 | 10 | 6 | 5 | **6.2** |
| [UniMath](formal-libraries/unimath.md) | 5 | 4 | 10 | 4 | 8 | **6.2** |
| [Lean 4 Core](formal-libraries/lean4-core.md) | 4 | 4 | 10 | 6 | 5 | **5.8** |

## Benchmarks & Evaluation Sets

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [LeanDojo Benchmark](benchmarks/leandojo-benchmark.md) | 8 | 8 | 10 | 9 | 7 | **8.4** |
| [MiniF2F](benchmarks/minif2f.md) | 6 | 3 | 9 | 9 | 8 | **7.0** |
| [FIMO](benchmarks/fimo.md) | 3 | 2 | 9 | 7 | 10 | **6.2** |
| [ProofNet](benchmarks/proofnet.md) | 5 | 3 | 8 | 8 | 6 | **6.0** |

## Autoformalization Datasets

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [MMA](autoformalization/mma.md) | 8 | 6 | 7 | 7 | 6 | **6.8** |
| [LEGO-Prover](autoformalization/lego-prover.md) | 6 | 6 | 9 | 6 | 6 | **6.6** |
| [MATH-to-Lean](autoformalization/math-to-lean.md) | 6 | 5 | 7 | 7 | 6 | **6.2** |
| [AutoFormalization (He et al.)](autoformalization/autoformalization-he-et-al.md) | 5 | 4 | 7 | 6 | 5 | **5.4** |

## Synthetic & Generated Corpora

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [Big-Math-RL-Verified](synthetic/big-math-rl-verified.md) | 8 | 10 | 7 | 8 | 7 | **8.0** |
| [Hypertree Proof Search Data](synthetic/hypertree-proof-search.md) | 7 | 6 | 8 | 5 | 7 | **6.6** |
| [Draft-Sketch-Prove](synthetic/draft-sketch-prove.md) | 6 | 5 | 7 | 6 | 6 | **6.0** |

## Human-Authored Reference Datasets

| Dataset | Diversity | Size | Formalization | Ease of Use | Complexity | **Overall** |
|---------|-----------|------|---------------|-------------|------------|-------------|
| [MATH](human-authored/math.md) | 7 | 6 | 1 | 9 | 7 | **6.0** |
| [Lean Workbook](human-authored/lean-workbook.md) | 7 | 7 | 5 | 7 | 6 | **6.4** |
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
| 5 | MiniF2F | 7.0 |
| 6 | HOL Light | 6.8 |
| 7 | MMA | 6.8 |
| 8 | LEGO-Prover | 6.6 |
| 9 | Hypertree Proof Search Data | 6.6 |
| 10 | Lean Workbook | 6.4 |
| 11 | Coq Standard Library | 6.2 |
| 12 | UniMath | 6.2 |
| 13 | FIMO | 6.2 |
| 14 | MATH-to-Lean | 6.2 |
| 15 | MATH | 6.0 |
| 16 | ProofNet | 6.0 |
| 17 | Draft-Sketch-Prove | 6.0 |
| 18 | Lean 4 Core | 5.8 |
| 19 | NaturalProofs | 5.8 |
| 20 | AMPS | 5.6 |
| 21 | AutoFormalization (He et al.) | 5.4 |
| 22 | GSM8K | 4.2 |
