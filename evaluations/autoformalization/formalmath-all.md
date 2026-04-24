# FormalMATH-All

**Category:** Autoformalization Datasets
**Link:** https://huggingface.co/datasets/SphereLab/FormalMATH-All

## Description

A collection of 5,560 mathematical competition problems autoformalized into Lean 4 by CUHK SphereLab. Problems are drawn from eight competition sources (AMC, AIME, MATH, Chinese competitions, and others), span 802 mathematical subdomains, and include compiler validation feedback for each formalized statement. Bilingual coverage (English and Chinese) makes it distinctive among competition autoformalization datasets.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 7 |
| Size | 5 |
| Level of Formalization | 8 |
| Ease of Use | 7 |
| Complexity | 8 |
| **Overall** | **7.0** |

## Justification

### Data Diversity (7/10)
Covers 802 labeled subdomains across algebra, number theory, geometry, combinatorics, analysis, and trigonometry. Eight distinct competition sources add breadth, and bilingual (EN/ZH) content is rare in this space. Scope is still bounded to competition mathematics — no library-style or research-level theorems.

### Size (5/10)
5,560 examples is moderate. Larger than most competition-focused formal datasets (e.g., FIMO, lean-math-formal-corpus), but small relative to Mathlib-scale corpora or Big-Math-RL-Verified. Adequate for fine-tuning autoformalization models but not for large-scale pretraining.

### Level of Formalization (8/10)
Each problem includes a Lean 4 autoformalization with compiler feedback indicating whether it compiled successfully. This is a meaningful quality signal — failures are flagged rather than silently included. However, "compiled" is a lower bar than "proven": statements may be syntactically valid but unprovable, and proof attempts are not uniformly verified.

### Ease of Use (7/10)
Available on HuggingFace in structured JSON with clear fields: problem statement, theorem name, autoformalization, compiler feedback, domain label, and solution. The compiler feedback boolean makes quality filtering trivial. Bilingual content adds slight complexity for English-only pipelines.

### Complexity (8/10)
Drawn from AMC/AIME/MATH and Chinese competition problems — solid competition-level mathematics. The upper tail (AIME, CMO) reaches genuine olympiad difficulty. Harder on average than most autoformalization datasets.
