# Agent Scaffolding Handoff

> Continuation brief for an assistive agent working on the Fibonacci OS
> repository.

## Purpose

This document explains the next phase of work for Fibonacci OS: creating the
initial `agents/` directory and scaffolding the project's role-based agent
system.

The repository has already been seeded with the foundational documentation under
`docs/`.

Before making changes, read:

1. `AGENTS.md`
2. `README.md`
3. `docs/philosophy.md`
4. `docs/constitution.md`
5. `docs/vision.md`
6. `docs/architecture.md`
7. `docs/workspace.md`
8. `docs/agents.md`
9. `docs/workflows.md`
10. `docs/roadmap.md`
11. `docs/glossary.md`

These documents are the current source of truth.

---

## Current Direction

Fibonacci OS treats agents as **specialised operating-system roles**, not
exclusively as AI personalities or vendor-specific assistants.

A role may eventually be implemented by:

- a human
- a language model
- a deterministic software service
- an automated workflow
- a combination of humans and software

The role specification must therefore remain independent of any particular
runtime.

ChatGPT Workspace Agents, Claude, Slack-like platforms, command-line tools, and
custom applications are all possible deployment environments. None should define
the core architecture.

---

## Objective and Status

The initial `agents/` directory and canonical specifications for all seven
roles are now complete:

1. Fibonacci Facilitator (`agents/facilitator/`)
2. Opportunity Scout (`agents/opportunity-scout/`)
3. Skeptical Analyst (`agents/skeptical-analyst/`)
4. Financial Controller (`agents/financial-controller/`)
5. Ethics Steward (`agents/ethics-steward/`)
6. Portfolio Steward (`agents/portfolio-steward/`)
7. Archivist (`agents/archivist/`)

Remaining documentation tasks include runtime-specific deployment guides
(such as `chatgpt.md`, `claude.md`, and `team-chat.md` under
`agents/facilitator/deployments/`).

The immediate objective remains documentation and structure, not runtime
orchestration software.

Do not build agent orchestration software yet.

---

## Recommended Directory Structure

Create:

```text
agents/
├── README.md
│
├── facilitator/
│   ├── README.md
│   ├── instructions.md
│   ├── evaluation.md
│   ├── examples/
│   │   └── README.md
│   └── deployments/
│       ├── README.md
│       ├── chatgpt.md
│       ├── claude.md
│       └── team-chat.md
│
├── opportunity-scout/
│   ├── README.md
│   ├── instructions.md
│   ├── evaluation.md
│   ├── examples/
│   │   └── README.md
│   └── deployments/
│       └── README.md
│
├── skeptical-analyst/
│   ├── README.md
│   ├── instructions.md
│   ├── evaluation.md
│   ├── examples/
│   │   └── README.md
│   └── deployments/
│       └── README.md
│
├── financial-controller/
│   ├── README.md
│   ├── instructions.md
│   ├── evaluation.md
│   ├── examples/
│   │   └── README.md
│   └── deployments/
│       └── README.md
│
├── ethics-steward/
│   ├── README.md
│   ├── instructions.md
│   ├── evaluation.md
│   ├── examples/
│   │   └── README.md
│   └── deployments/
│       └── README.md
│
├── portfolio-steward/
│   ├── README.md
│   ├── instructions.md
│   ├── evaluation.md
│   ├── examples/
│   │   └── README.md
│   └── deployments/
│       └── README.md
│
└── archivist/
    ├── README.md
    ├── instructions.md
    ├── evaluation.md
    ├── examples/
    │   └── README.md
    └── deployments/
        └── README.md
```

This structure may be simplified if the empty directories create unnecessary
noise, but preserve the conceptual separation between:

- role specification
- behavioural instructions
- evaluation
- examples
- runtime-specific deployment guidance

---

## Directory Responsibilities

### `agents/README.md`

Create an index and overview of the agent system.

It should explain:

- what an agent means in Fibonacci OS
- why agents are modelled as roles
- the difference between a role and its implementation
- the human decision-making model
- how the roles collaborate
- how new roles may be introduced
- how deployment-specific instructions are separated from canonical
  specifications

Include a concise collaboration diagram.

Suggested flow:

```text
Human
  │
  ▼
Fibonacci Facilitator
  │
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

Make clear that actual workflows may involve only a subset of roles.

---

### Role `README.md`

Each role directory must contain a canonical role specification.

Use the same headings for every role:

```markdown
## Role Name

### Mission

### Purpose

### Responsibilities

### Inputs

### Outputs

### Jurisdiction

### Constraints

### Collaboration

### Escalation

### Success Criteria

### Failure Modes

### Example Activities

### Implementation Independence
```

The specification must describe **what the role is**, not how a particular model
should be prompted.

---

### `instructions.md`

This file should contain behavioural guidance suitable for adapting into an AI
system prompt or Workspace Agent instruction set.

Use headings such as:

```markdown
## Role Name Instructions

### Role

### Operating Principles

### Working Method

### Required Behaviours

### Prohibited Behaviours

### Output Expectations

### Handling Uncertainty

### Human Approval Requirements
```

Instructions should be:

- concise
- operational
- testable
- compatible with different language models
- grounded in the Fibonacci OS Constitution

Do not include vendor-specific tool syntax in the canonical instructions.

---

### `evaluation.md`

Define how the quality of the role's work can be assessed.

Include:

```markdown
## Role Name Evaluation

### Evaluation Goals

### Quality Criteria

### Pass Conditions

### Warning Signs

### Failure Conditions

### Test Scenarios
```

Prefer observable criteria.

Avoid vague statements such as:

> The response should be good.

Prefer criteria such as:

> The response distinguishes evidence, assumptions, and speculation.

or:

> The role identifies at least one material risk before recommending further
> investment.

Evaluation should cover both task quality and constitutional alignment.

---

### `examples/`

Initially, create only an explanatory `README.md` unless strong examples can be
written without inventing project context.

Explain that future examples may contain:

- sample inputs
- expected outputs
- poor outputs with commentary
- disagreement between roles
- human escalation examples
- completed workflow artefacts

Avoid treating examples as rigid templates unless the format is intentionally
normative.

---

### `deployments/`

Deployment files describe how a canonical role should be adapted for a
particular environment.

They must not redefine the role.

The deployment layer may describe:

- invocation style
- response length
- supported tools
- connected knowledge sources
- approval rules
- channel behaviour
- memory policy
- formatting expectations
- runtime limitations

A deployment must remain subordinate to:

1. the Constitution
2. the canonical role specification
3. the canonical behavioural instructions

---

## Platform Independence

The user currently works with both ChatGPT and Claude on desktop.

They are also considering open-source team-chat or Slack-like platforms,
including:

- Rocket.Chat
- Zulip
- Buzz.xyz
- other self-hosted or federated collaboration systems

No platform has been selected.

For that reason, avoid assumptions such as:

- agents will always communicate through Slack threads
- agents can invoke one another directly
- every runtime supports persistent memory
- every runtime supports shared files
- every runtime supports synchronous orchestration
- every runtime exposes the same tool or approval model

Use the generic term **team-chat deployment** where platform-neutral guidance is
sufficient.

Platform-specific files can be added later when a runtime is selected and
tested.

---

## The Fibonacci Facilitator

The Facilitator is the highest-priority role because it connects the specialist
roles into a coherent user experience.

Its mission is to:

- understand the user's objective
- select an appropriate workflow
- identify which specialist roles are relevant
- frame clear questions for those roles
- preserve shared context
- surface disagreement
- synthesise findings
- identify decisions requiring human judgement
- coordinate final documentation

The Facilitator is not a manager with authority over the human.

It may coordinate analysis but may not make consequential decisions on the
user's behalf.

### Facilitator Jurisdiction

The Facilitator may:

- choose a suitable workflow
- request specialist perspectives
- sequence analysis
- summarise evidence
- compare recommendations
- identify unresolved questions
- recommend next actions
- request human decisions
- hand completed decisions to the Archivist

The Facilitator may not:

- conceal disagreement
- override an ethical objection without explanation
- fabricate specialist conclusions
- authorise spending
- publish externally
- commit the user to a venture
- present recommendations as human decisions
- claim that independent agents were consulted when only one model simulated the
  roles

That final distinction is important.

If a single model performs several roles, it must describe the result as a
**multi-role analysis**, not falsely imply that independent systems reviewed the
work.

---

## Initial Role Intent

Use the following as the starting point for each specification.

### Opportunity Scout

Identifies unmet needs, emerging opportunities, relevant signals, and testable
possibilities.

It should generate hypotheses rather than declare that an opportunity is proven.

### Skeptical Analyst

Challenges assumptions, identifies weak evidence, explores counterarguments, and
tests whether a proposal survives critical examination.

It should improve decisions without becoming reflexively negative.

### Financial Controller

Examines cost, affordability, financial risk, sustainability, cash implications,
and the economics of proposed experiments.

It advises but does not approve expenditure.

### Ethics Steward

Examines potential harm, fairness, privacy, accessibility, power, consent,
vulnerable groups, environmental consequences, and alignment with the
Constitution.

Material ethical concerns must be surfaced clearly rather than softened for
convenience.

### Portfolio Steward

Evaluates how a proposed project fits with existing work, capacity, strategy,
dependencies, opportunity cost, and long-term portfolio health.

It should discourage unmanaged project accumulation.

### Archivist

Preserves decisions, evidence, assumptions, outcomes, lessons, and reusable
knowledge.

It should distinguish current guidance from historical records and avoid
silently rewriting prior decisions.

### Fibonacci Facilitator

Coordinates the roles and presents their work as a coherent decision-support
process.

---

## Jurisdiction Model

Every role specification must distinguish between:

- what the role may observe
- what the role may analyse
- what the role may recommend
- what the role may modify
- what requires human approval

Use this general principle:

```text
Agents may analyse and advise.
Humans retain authority for consequential decisions.
```

Do not grant roles broad write, publication, purchasing, deletion, or
communication authority by default.

---

## Collaboration Rules

Roles should not be forced into artificial consensus.

When roles disagree:

1. preserve the disagreement
2. identify its cause
3. identify the evidence needed to resolve it
4. explain the consequence of each interpretation
5. return the unresolved choice to the human where appropriate

The Facilitator should synthesise without erasing dissent.

The Ethics Steward should not be treated as a ceremonial final check.

The Skeptical Analyst should not be allowed to block all experimentation merely
because uncertainty remains.

The Financial Controller should distinguish between financial risk and total
value.

The Opportunity Scout should not treat enthusiasm as validation.

The Portfolio Steward should consider capacity and opportunity cost.

The Archivist should record both the decision and its rationale.

---

## Suggested Workflow for This Scaffolding Task

Proceed in this order:

1. Review the existing documentation.
2. Create `agents/README.md`.
3. Create the `facilitator/` specification.
4. Create the remaining canonical role specifications.
5. Create all `instructions.md` files.
6. Create the evaluation files.
7. Add minimal example-directory guidance.
8. Add deployment guidance.
9. Review terminology against `docs/glossary.md`.
10. Review all files against `docs/constitution.md`.
11. Update repository navigation where appropriate.

Do not create large amounts of boilerplate merely to fill the directory.

Prefer concise, meaningful documents.

---

## Repository Updates

After scaffolding the directory, consider updating:

### Root `README.md`

Add a link to `agents/README.md`.

### `docs/agents.md`

Confirm that it points readers to the canonical role specifications under
`agents/`.

### `docs/architecture.md`

Add or verify the distinction between:

- role definitions
- orchestration
- deployment environments
- user-facing conversation surfaces

### `docs/glossary.md`

Add definitions if they are not already present for:

- Facilitator
- Jurisdiction
- Orchestration
- Deployment
- Runtime
- Multi-role analysis

Do not introduce duplicate terminology unnecessarily.

---

## Out of Scope

Do not yet implement:

- an agent framework
- an orchestration server
- model-to-model messaging
- Slack bots
- Rocket.Chat bots
- Zulip bots
- API integrations
- persistent memory services
- vector databases
- workflow automation
- autonomous decision-making
- vendor-specific configuration schemas

These may follow after the role model has been exercised manually.

---

## First Practical Milestone

The first milestone is complete when:

- every initial role has a canonical specification
- every role has behavioural instructions
- every role has evaluation criteria
- the Facilitator can conceptually coordinate the other roles
- role jurisdiction is explicit
- no file depends on a specific vendor
- ChatGPT and Claude deployments could both be derived from the documentation
- a future team-chat deployment could be added without changing the canonical
  roles

---

## Recommended First Prototype

After role specifications are established, prepare a manual prototype of the
Fibonacci Facilitator.

The prototype can exercise an illustrative linear review workflow:

```text
Opportunity
    ↓
Critical review
    ↓
Ethical review
    ↓
Financial review
    ↓
Portfolio review
    ↓
Human decision
    ↓
Archive
```

This may initially run:

- inside one ChatGPT Workspace Agent
- inside one Claude project or equivalent configuration
- through manually invoked specialist agents
- as a single-model multi-role analysis

The repository specifications must remain valid across all four approaches.

---

## Working Style

When continuing this work:

- preserve the existing documentation style
- use clear Markdown headings
- prefer direct prose over jargon
- keep documents implementation-independent
- explain significant architectural choices
- distinguish current decisions from future possibilities
- avoid overstating what any platform currently supports
- do not fabricate repository contents
- inspect existing files before changing them
- keep human authority explicit

---

## Completion Report

When the scaffolding work is complete, provide a concise report containing:

1. files created
2. files modified
3. architectural decisions made
4. assumptions introduced
5. unresolved questions
6. recommended next step

Do not proceed into runtime implementation unless explicitly asked.
