# System Prompts

This directory contains persona-based system prompts for interacting with the datasets catalogued in this repository. Each prompt is designed to configure an AI assistant to respond in a way that is appropriate for a specific type of user — matching their mathematical background, goals, and the vocabulary they are likely to use.

## Purpose

The same verified math dataset means something very different depending on who is asking about it. A Lean tactic trace is a training signal to an ML researcher, a learning resource to a PhD student, and an incomprehensible wall of symbols to a middle schooler. These prompts encode that context so that an AI assistant can give useful, calibrated responses without requiring the user to explain themselves every time.

## How to use

Paste the contents of the relevant `.md` file as the **system prompt** when initializing a conversation with an AI assistant (e.g., Claude, GPT-4). The user can then ask questions about any dataset in this repository — what it contains, how to use it, whether it fits their use case — and the assistant will respond in a register appropriate for that persona.

Most API and chat interfaces support a system prompt field. In Claude's API this is the `system` parameter; in OpenAI's it is the `messages` array entry with `role: "system"`.

## Personas

| File | Persona | Best for |
|---|---|---|
| `terence-tao.md` | Terence Tao | Expert research mathematician exploring formalization and AI-assisted discovery |
| `phd-math-student.md` | PhD math student | Graduate researcher new to proof assistants, looking for practical entry points |
| `undergraduate-student.md` | Undergraduate student | Math/CS undergrad encountering formal verification for the first time |
| `ai-researcher-model-developer.md` | AI researcher / model developer | ML practitioner evaluating datasets for training or benchmarking |
| `software-engineer-ai-math-curious.md` | Software engineer | Engineer who wants to build with or understand these datasets pragmatically |
| `middle-school-math-prodigy.md` | Middle school math prodigy | Young competition mathematician exploring math and AI out of curiosity |

## Adding a new persona

Each prompt follows a consistent structure:
1. **Who you are talking to** — background, knowledge level, motivation
2. **Goals** — what this user is actually trying to accomplish with the datasets
3. **Tone and interaction style** — how to communicate with them
4. **What to avoid** — failure modes to prevent

To add a new persona, create a new `.md` file following that structure and add a row to the table above.
