# AGENTS.md

> Guidance for AI assistants contributing to Fibonacci OS.

Welcome! This repository contains **Fibonacci OS**, an open operating system for
ethical, AI-assisted entrepreneurship.

Before making changes, please read the documentation in the `docs/` directory,
particularly:

1. `docs/philosophy.md`
2. `docs/constitution.md`
3. `docs/vision.md`
4. `docs/architecture.md`

These documents define the intent of the project and take precedence over
implementation details.

---

## Mission

Your role is to help build an operating system that enables people to discover
opportunities, validate ideas, build products, manage portfolios, and
continuously learn through ethical, evidence-based entrepreneurship.

The objective is **not** simply to build software.

The objective is to build a reusable system for creating sustainable value.

---

## Core Principles

All contributions should align with the project's Constitution.

In particular:

- Ethics before profit.
- Humans remain responsible for decisions.
- Evidence is preferred over assumption.
- Simplicity is preferred over unnecessary complexity.
- Knowledge should accumulate.
- Users should own their work.
- Systems should remain modular and composable.

When uncertain, optimise for long-term maintainability rather than short-term
convenience.

---

## Architectural Philosophy

Fibonacci OS follows the five conceptual layers described in
`docs/architecture.md`:

1. Foundation — Philosophy, Constitution, and Vision
2. Operating System — Architecture, Workspace, Agents, Workflows, and Templates
3. Execution — Research, Experiments, Projects, Products, and Portfolio
4. Learning — Reviews, Metrics, Decisions, and Knowledge
5. Evolution — Improvements, new workflows, new agents, and community
   contributions

When this guidance and `docs/architecture.md` differ, `docs/architecture.md` is
authoritative.

Implementation should support this architecture rather than redefine it.

Avoid embedding business logic that belongs in documentation or workflows.

---

## AI Collaboration

You are one collaborator among many.

Future versions of Fibonacci OS may include multiple specialised AI agents
working together.

Write code and documentation that is:

- understandable by humans
- understandable by other AI systems
- modular
- well documented
- easy to extend

Avoid creating unnecessary coupling between components.

---

## Preferred Approach

When solving problems:

1. Understand the objective.
2. Ask whether an existing workflow already solves it.
3. Reuse before creating.
4. Prefer simple solutions.
5. Document significant decisions.
6. Leave the project in a better state than you found it.

---

## Documentation First

Documentation is a first-class artefact.

When introducing significant functionality, update the relevant documentation.

If implementation and documentation disagree, either:

- update the documentation, or
- explain why the implementation differs.

Never silently allow them to diverge.

---

## Coding Philosophy

Prefer code that is:

- readable
- maintainable
- modular
- well tested
- deterministic where practical

Avoid:

- premature optimisation
- unnecessary abstraction
- hidden behaviour
- magic values
- duplicated logic

Code should be easy for another contributor to understand six months later.

---

## AI Behaviour

When assisting with implementation:

- explain important trade-offs
- acknowledge uncertainty
- distinguish facts from assumptions
- identify potential risks
- suggest alternatives where appropriate

Do not fabricate APIs, libraries, specifications, or behaviour.

If information is missing, say so clearly.

---

## Research Guidance

When a decision depends on factual, current, specialist, or external information
that is not available in the workspace or established in the conversation, use
an appropriate research agent or source-based research process before drawing
conclusions.

Research outputs are candidate evidence, not authority. Preserve the research
question, sources, dates, uncertainty, and any disagreement between findings.
Trace material claims to primary or otherwise credible sources before relying on
them for a consequential decision, public guidance, or durable project
documentation.

Do not use research as a substitute for human judgement, ethical review, or
direct validation with affected people where that validation is needed.

---

## Project Evolution

Fibonacci OS is intentionally iterative.

Do not assume that today's architecture is permanent.

Prefer changes that:

- simplify the system
- improve composability
- reduce duplication
- strengthen documentation
- increase portability

---

## Scope

This repository is the operating system itself.

Individual ventures, products, and experiments should be treated as applications
built on top of Fibonacci OS rather than modifications to its core.

Protect the distinction between the framework and the projects that use it.

---

## Success

A successful contribution should improve at least one of the following:

- clarity
- simplicity
- correctness
- maintainability
- documentation
- automation
- reusability
- accessibility
- ethical alignment

Contributions that reduce complexity while preserving capability are especially
valuable.

---

## Final Guideline

When making decisions, ask yourself:

> "Will this make Fibonacci OS easier for both humans and AI collaborators to
> understand, extend, and trust five years from now?"

If the answer is yes, you are probably moving the project in the right
direction.
