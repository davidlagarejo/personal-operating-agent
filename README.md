# DavidSan

Your privacy-first AI agent for professional positioning and high-priority execution.

`DavidSan` is a larger personal AI project built around a fine-tuned `Phi-4` model, privacy-aware context handling, and execution workflows that help turn scattered information into clear positioning and concrete next actions.

This repository is the public-facing version of that system: a clean technical foundation, early package structure, tests, documentation, and contribution scaffolding for building in the open.

## Demo

This public repo now includes an English dashboard demo based on the real interaction model behind `DavidSan`.

- dashboard demo: [examples/dashboard-demo.html](examples/dashboard-demo.html)
- dashboard notes: [docs/dashboard.md](docs/dashboard.md)
- architecture overview: [docs/architecture.md](docs/architecture.md)

The demo is intentionally lightweight, but it shows the shape of the product:

- a priority-driven workspace instead of a flat chat
- proactive questioning from the model when key context is missing
- rationale, fit scoring, and references behind recommendations
- a timeline layer that keeps execution centered on what matters most

## Why This Project Exists

Most AI writing tools help people write faster.

Far fewer help people represent themselves better.

`DavidSan` explores a different direction: an assistant that helps a person articulate what they do, how they think, why they create value, and what they should do next, while staying privacy-aware by design.

## What Problem It Tries To Solve

This project is built around a practical gap:

- people often have strong experience but weak positioning
- valuable context is usually fragmented across notes, drafts, bios, and conversations
- existing tools often optimize for generic output rather than authentic representation
- personal AI workflows can easily become privacy leaks if they depend on exposing raw context

`DavidSan` is meant to help transform context into usable professional narrative with more clarity and less overexposure.

## What Makes This System Different

`DavidSan` is not just a prompt wrapper.

The larger project combines:

- a fine-tuned `Phi-4` model
- direct-questioning behavior to proactively understand the user
- contextual file reading to build better working knowledge
- `n8n` workflows for execution-oriented tasks
- a dashboard designed around priorities, rationale, and follow-through

This makes the system closer to a personal operating layer than a generic assistant.

## Recruiter-Oriented Framing

For recruiters, hiring managers, and technical reviewers, this repository shows more than a prototype idea.

It demonstrates:

- product thinking around a concrete user problem
- practical interest in privacy-aware AI workflows
- early system design around a fine-tuned LLM-based assistant
- willingness to publish work-in-progress transparently
- the ability to structure a project so it can grow into a usable product

Even at an early stage, the repo communicates how I think about AI tooling: not just generation, but representation, control, and trust.

## Current Scope

The public repo currently includes:

- a minimal Python package in `src/davidsan`
- reproducible project setup in `pyproject.toml`
- smoke tests for a clean baseline
- folders prepared for prompts, examples, scripts, configs, and docs
- contribution and community files for open collaboration

This is not the full agent yet. It is the public, reviewable foundation of the project.

## Core Direction

`DavidSan` is being shaped as an assistant that:

- helps express a person's value more clearly
- uses a fine-tuned `Phi-4` model for generation and reformulation
- relies on intentionally selected context instead of indiscriminate data ingestion
- asks direct questions to understand missing context proactively
- reads relevant user files to ground its reasoning
- supports execution through workflow orchestration
- treats privacy as a design constraint, not an afterthought
- can evolve into a transparent, auditable personal AI workflow

## Fine-Tuned Phi-4 And Execution Layer

At the core of the larger project is a fine-tuned `Phi-4` model shaped to prioritize proactive understanding of the user.

That means the agent is designed to:

- ask direct questions when context is missing
- learn from relevant user files instead of relying only on one-shot prompting
- reason about priorities rather than simply answer requests
- move from conversation into execution-oriented assistance

Alongside the model, `n8n` is used as an orchestration layer for targeted workflows such as:

- continuous research and monitoring
- task prioritization
- argumentation and reasoning support
- email drafting
- personal CRM follow-up
- dashboard updates and operational flows

## What Is Public And What Is Not

This repository is intentionally selective.

Public:

- project structure
- package code
- tests
- public documentation
- non-sensitive prompts and configuration patterns
- roadmap direction and open design thinking

Not public:

- real personal data
- private conversations or identifiable histories
- secrets, tokens, or `.env` files
- local usage configuration tied to a personal workflow
- any memory layer or operating context that would expose sensitive information

## Repository Layout

| Folder | Purpose |
|---|---|
| `src/` | Core package source |
| `tests/` | Baseline validation |
| `docs/` | Technical and product notes |
| `scripts/` | Project utilities |
| `prompts/` | Prompt templates and experiments |
| `configs/` | Safe public configuration |
| `examples/` | Future anonymized demos |

## Dashboard And Timeline

An important part of the larger `DavidSan` system is the dashboard layer.

The dashboard is designed to keep work grounded in priority, context, and action rather than treating everything as a flat chat history or generic task list.

It is meant to surface:

- what should be done first
- why it matters
- how well a task fits the current goals
- what evidence or references support the recommendation
- what the next action should be

The timeline is especially important.

It helps maintain focus on the highest-priority work, makes sequencing and deadlines visible, reduces drift, and prevents strategically important tasks from being buried under reactive noise.

This matters because the product is not only trying to generate good language. It is trying to keep the user oriented toward the highest-value next move.

## Run Locally

```bash
python3.12 -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
pytest
```

## Why It Matters As A Public Project

This repo is not meant to be performative open source.

It is meant to show:

- a real project with a specific use case
- a privacy-aware AI product direction
- fine-tuning and orchestration thinking, not just prompt experimentation
- a technical foundation that can be inspected and extended
- an honest early-stage build rather than a polished but shallow demo

That makes it useful both as a community-facing repository and as a signal of technical/product capability.

## Current Status

Today, the public version includes:

- package scaffold
- initial test coverage
- public documentation
- contribution standards
- basic architecture notes

Next logical steps:

- add real assistant modules
- define input and output contracts
- include safe prompt examples
- document more of the fine-tuned `Phi-4` interaction model
- expose more of the execution workflow design
- turn more of the dashboard behavior into reproducible public demos
- add a lightweight privacy and review layer

## Open Roadmap

Feedback is especially welcome on:

- agent flow design
- prompt structure and evaluation
- privacy boundaries and sanitization
- product positioning for professional storytelling
- packaging this into a more reusable assistant workflow

## Community

Suggestions, issues, and pull requests are welcome.

Please review [CONTRIBUTING.md](CONTRIBUTING.md), [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md), and [SECURITY.md](SECURITY.md) before contributing.

## License

Released under the MIT License. See [LICENSE](LICENSE).
