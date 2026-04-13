# Contributing to awesome-verified-math-data

Thank you for helping grow this resource. The goal is to maintain a high-quality, accurate list of verified mathematical datasets — so curation matters more than comprehensiveness. Please read these guidelines before submitting.

---

## What belongs here

This list is focused on **formally verified** mathematical data: corpora whose correctness has been checked by a proof assistant (Lean, Coq, Isabelle, HOL Light, Metamath, etc.).

A contribution is a good fit if it is one of the following:

- A **formal library** — a body of machine-checked mathematics
- A **benchmark or evaluation set** — problems with formal statements or verified solutions
- An **autoformalization dataset** — paired informal/formal mathematical content
- A **synthetic corpus** — machine-generated, formally verified data
- A **tool or infrastructure project** — software for extracting, processing, or interacting with formal math data
- An **informal reference dataset** — unverified but widely used (clearly labeled as such)

If you are unsure whether something fits, open an issue and ask before submitting a PR.

---

## What does not belong here

- Informal math datasets without any formal verification component (unless they are significant reference datasets added to the "Human-Authored Reference" section)
- Paywalled or access-restricted datasets with no public version
- Preprints describing a dataset that has not yet been publicly released
- General math AI papers not accompanied by a released dataset or tool
- Unmaintained or broken links (check before submitting)

---

## How to submit

1. **Fork** this repository and create a new branch.
2. Add your entry to the appropriate section in `README.md`.
3. Follow the entry format (see below).
4. Open a **pull request** with a short description of what you are adding and why it belongs.

For larger changes — new sections, reorganization, changes to scope — please open an **issue** first to discuss before putting in the work.

---

## Entry format

Each entry should follow this pattern:

```
- **[Name](url)** — One or two sentences describing what it is, what proof assistant it uses (if applicable), and its approximate scale or scope.
```

Keep descriptions factual and neutral. Avoid promotional language. If the dataset has an associated paper, you may link to it parenthetically at the end of the description.

**Example:**

```
- **[MiniF2F](https://github.com/openai/miniF2F)** — 488 competition-level math problems formalized in Lean, Isabelle, HOL Light, and Metamath. The standard benchmark for evaluating formal theorem proving systems.
```

---

## Quality checklist

Before submitting, please verify:

- [ ] The link is working and points to the correct resource
- [ ] The dataset or tool is publicly accessible (no login required to access the core resource)
- [ ] The description is accurate and in your own words (not copied from the project's own README)
- [ ] For verified datasets: the data is formally checked by a proof assistant, not just claimed to be correct
- [ ] The entry is placed in the most appropriate section
- [ ] The entry is in alphabetical order within its section (preferred, not required)

---

## Updating or removing entries

If you find a broken link, an inaccurate description, or a dataset that has been taken down, please open a pull request or issue. Keeping existing entries accurate is just as valuable as adding new ones.

---

## Code of conduct

Be respectful. Disagreements about what belongs in the list should be resolved in issues, not PRs. The maintainer has final discretion on all curation decisions.
