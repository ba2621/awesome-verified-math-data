# NuminaMath-CoT

**Category:** Human-Authored Reference Datasets
**Link:** https://huggingface.co/datasets/AI-MO/NuminaMath-CoT

## Description

860,000 competition mathematics problems with chain-of-thought solutions, sourced from Chinese high school math competitions, AMC/AIME, Olympiad archives, and other international competitions. Produced by the Numina team for the first AI Mathematical Olympiad (AIMO) Prize competition, which it won. Not formally verified, but solutions are human-curated and filtered for correctness. A standard reference dataset for RL-based math training.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 8 |
| Size | 10 |
| Level of Formalization | 1 |
| Ease of Use | 9 |
| Complexity | 7 |
| **Overall** | **7.0** |

## Justification

### Data Diversity (8/10)
Aggregates problems from AMC 8/10/12, AIME, MATH, Chinese high school and competition problems (CNMO, CMO), and international olympiad archives across multiple countries. Broad coverage of competition styles and problem types. Diversity within the competition math domain is excellent; no formal library or graduate-level mathematics.

### Size (10/10)
860,000 problems — one of the largest open-source math problem datasets available. Paired with full chain-of-thought solutions. The scale is what makes this valuable for RL training; it provides enough coverage of competition math problem space to train general reasoning without rapid saturation.

### Level of Formalization (1/10)
No formal verification. Solutions are human-written chain-of-thought, not machine-checkable proofs. The dataset was curated and filtered by humans but remains informal natural language. A score of 1 rather than 0 reflects that the solutions are held to a correctness standard higher than raw scraping.

### Ease of Use (9/10)
Available on HuggingFace with excellent documentation and a clean, standard format. No special tooling required. The dataset has been widely adopted in the open-source RL math training community since the AIMO competition, meaning there is abundant example code and pipelines available.

### Complexity (7/10)
Spans a wide difficulty range, from AMC 8 (accessible middle school) through IMO and national olympiad problems. The upper tail is genuinely hard competition mathematics. Average complexity across the full dataset is moderate-to-high; the distribution is heavily skewed toward Chinese high school competition problems, which sit at AMC–AIME difficulty.
