# GSM8K

**Category:** Human-Authored Reference Datasets
**Link:** https://github.com/openai/grade-school-math

## Description

8,500 grade-school math word problems from OpenAI, each with a step-by-step natural language solution. Designed to test multi-step reasoning in LLMs on elementary arithmetic and basic problem-solving. Widely used in early chain-of-thought research.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 3 |
| Size | 5 |
| Level of Formalization | 1 |
| Ease of Use | 10 |
| Complexity | 2 |
| **Overall** | **4.2** |

## Justification

### Data Diversity (3/10)
Restricted to grade-school arithmetic word problems — addition, subtraction, multiplication, division, and simple rate/ratio reasoning. Extremely narrow mathematical scope by design. Not representative of the mathematical breadth relevant to formal verification research.

### Size (5/10)
8,500 problems is reasonable for a benchmark but modest in scale. The problems are human-authored and quality-controlled, which limits how far the dataset can be expanded.

### Level of Formalization (1/10)
Entirely informal natural language. No formal verification. Included as a reference for the broader math AI ecosystem; not relevant as a source of verified training data.

### Ease of Use (10/10)
The most accessible dataset on this list. Universally supported across all major evaluation frameworks. Available in multiple formats, trivially loadable, and requires no special tooling. The gold standard for ease of use.

### Complexity (2/10)
Grade-school level mathematics — elementary arithmetic, basic fractions, simple word problems. Modern LLMs achieve near-perfect accuracy, indicating the dataset is effectively saturated for current models. Very low complexity relative to the rest of this list.
