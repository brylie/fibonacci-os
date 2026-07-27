# Fibonacci OS Roles

> *Fibonacci OS roles provide implementation-independent decision support for ethical, evidence-based entrepreneurship.*

## What an Agent Means

In Fibonacci OS, an agent is a specialised operating-system role. The role describes a responsibility, not a personality, model, product, or vendor integration. A role may be performed by a human, language model, deterministic service, workflow, or combination of these.

Canonical role specifications are the source of truth. `instructions.md` describes observable behaviour, `evaluation.md` describes how work can be assessed, `examples/` contains learning material, and `deployments/` describes how a runtime may adapt the role. Deployment guidance must not redefine the role.

## Human Authority

Roles may observe, analyse, recommend, and request decisions. Humans remain responsible for goals, priorities, ethical judgement, consequential commitments, spending, publication, and irreversible actions.

## Initial Roles

| Role | Primary contribution |
| --- | --- |
| [Fibonacci Facilitator](facilitator/) | Coordinates roles and presents transparent decision support |
| [Opportunity Scout](opportunity-scout/) | Finds needs, signals, and testable possibilities |
| [Skeptical Analyst](skeptical-analyst/) | Challenges assumptions and identifies evidence gaps |
| [Financial Controller](financial-controller/) | Examines affordability, economics, and financial risk |
| [Ethics Steward](ethics-steward/) | Examines harm, rights, consent, and constitutional alignment |
| [Portfolio Steward](portfolio-steward/) | Evaluates capacity, opportunity cost, and portfolio health |
| [Archivist](archivist/) | Preserves decisions, evidence, outcomes, and reusable knowledge |

## Collaboration

```text
Human objective
      │
      ▼
Fibonacci Facilitator
      ├── Opportunity Scout
      ├── Skeptical Analyst
      ├── Ethics Steward
      ├── Financial Controller
      └── Portfolio Steward
      │
      ▼
Human decision
      │
      ▼
Archivist
```

Actual workflows should use only the roles relevant to the question. Roles may disagree; the Facilitator preserves the disagreement, its evidence, and the unresolved human choice. If one implementation performs several roles, it must call the result a multi-role analysis rather than imply independent review.

## Adding Roles

A new role should address a durable responsibility that is not already covered. Define its jurisdiction and relationship to existing roles before adding implementation details. New roles should include the same five document types used here and should be tested in a manual workflow before automation is considered.

## Current Boundary

This directory contains specifications only. It does not define an orchestration server, model-to-model messaging, persistent memory, vendor configuration, or autonomous decision-making.
