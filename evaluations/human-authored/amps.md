# AMPS

**Category:** Human-Authored Reference Datasets
**Link:** https://github.com/hendrycks/math

## Description

A large pretraining dataset combining Khan Academy problems and Mathematica-generated exercises. Used for pretraining the MATH dataset models. Covers a wide range of K-12 and early undergraduate mathematics in a procedurally generated format.

## Evaluation

| Factor | Score (1–10) |
|--------|-------------|
| Data Diversity | 6 |
| Size | 8 |
| Level of Formalization | 1 |
| Ease of Use | 8 |
| Complexity | 5 |
| **Overall** | **5.6** |

## Justification

### Data Diversity (6/10)
Khan Academy covers a broad K-12 curriculum across arithmetic, algebra, geometry, statistics, and calculus. Mathematica-generated problems add procedural variety. The combination is diverse at the elementary-to-undergraduate level but does not extend to research mathematics.

### Size (8/10)
One of the larger datasets on this list by problem count. The Mathematica generation component enables scale beyond what human curation alone can achieve, producing millions of problems across many topic areas.

### Level of Formalization (1/10)
Entirely informal. Problems and solutions are in natural language or symbolic notation without any formal verification. Included as a pretraining reference; not a source of verified mathematical data.

### Ease of Use (8/10)
Distributed alongside the MATH dataset, with clear documentation. Standard format, widely used in pretraining pipelines. The procedural generation aspect means the data is already structured and consistent.

### Complexity (5/10)
K-12 through early calculus level. Mathematica-generated problems can be algorithmically complex but rarely require deep mathematical insight. The upper end is approximately first-year undergraduate level — well below competition math or graduate mathematics.
