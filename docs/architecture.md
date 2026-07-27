# Architecture

> *Fibonacci OS is an operating system for entrepreneurial practice. Its architecture organises principles, knowledge, people, artificial intelligence, and work into a coherent system for creating sustainable value.*

This document describes the conceptual architecture of Fibonacci OS. It is intentionally independent of any programming language, software framework, or implementation.

---

# Architectural Principles

The architecture is guided by five principles:

- **Human-centred** — Humans define goals and make final decisions.
- **AI-assisted** — Artificial intelligence amplifies, but does not replace, human capability.
- **Evidence-driven** — Decisions are informed by observation, experimentation, and measurement.
- **Modular** — Components can evolve independently while remaining interoperable.
- **Composable** — Small, reusable building blocks create more capable systems.

---

# Layers of the Operating System

Fibonacci OS is organised into five conceptual layers.

```text
Purpose
│
├── Philosophy
├── Constitution
└── Vision
        │
        ▼
Operating System
│
├── Architecture
├── Workspace
├── Agents
├── Workflows
└── Templates
        │
        ▼
Execution
│
├── Research
├── Experiments
├── Projects
├── Products
└── Portfolio
        │
        ▼
Learning
│
├── Reviews
├── Metrics
├── Decisions
└── Knowledge
        │
        ▼
Evolution
│
├── Improvements
├── New Workflows
├── New Agents
└── Community Contributions
```

Each layer builds upon the one above it.

---

# Foundation Layer

The foundation defines **why** the operating system exists.

It consists of:

- **Philosophy** — the purpose of the project.
- **Constitution** — the enduring principles.
- **Vision** — the long-term direction.

These documents should change infrequently and guide every other architectural decision.

---

# Operating System Layer

This layer defines **how the system operates**.

It includes:

- workspace organisation
- AI agents
- shared artefacts
- reusable workflows
- templates
- documentation
- governance

This layer provides structure without dictating individual projects.

### Shared Artefacts

Shared artefacts are the human-readable documents exchanged between roles and workflow stages. They provide a stable language for collaboration without requiring a particular runtime or machine schema. Their canonical forms are defined in [`docs/artefacts.md`](artefacts.md).

---

# Execution Layer

This is where work happens.

Typical lifecycle:

```text
Opportunity
    ↓
Research
    ↓
Validation
    ↓
Experiment
    ↓
Prototype
    ↓
Product
    ↓
Operation
    ↓
Review
```

Every project progresses through some variation of this lifecycle.

Not every project reaches every stage.

Learning is considered a successful outcome regardless of commercial success.

---

# Learning Layer

Knowledge generated through execution is captured rather than discarded.

Examples include:

- experiment results
- customer feedback
- financial metrics
- technical discoveries
- design decisions
- reusable code
- documentation improvements

The operating system becomes more valuable as knowledge accumulates.

---

# Evolution Layer

Fibonacci OS continuously improves itself.

Learning produces:

- better templates
- improved workflows
- new AI agents
- clearer documentation
- refined practices
- stronger communities

Every completed project should strengthen the operating system for future projects.

---

# Core Components

The operating system consists of several interacting components.

## Workspace

The workspace stores all knowledge and project artefacts.

It provides a consistent organisational structure independent of software implementation.

---

## Agents

Agents define specialised operating-system roles. A role may be implemented by a human, AI system, deterministic service, workflow, or combination of these. The canonical role definition is independent of implementation.

Examples include:

- opportunity discovery
- research
- financial analysis
- technical architecture
- risk assessment
- documentation
- portfolio management

Agents collaborate rather than compete.

No single agent possesses complete authority.

Role definitions, orchestration, deployment environments, and user-facing conversation surfaces are separate concerns:

- **Role definition** describes mission, jurisdiction, responsibilities, inputs, outputs, and constraints.
- **Behavioural instructions** adapt a role into operational guidance without choosing a vendor.
- **Orchestration** sequences roles and preserves context for a workflow.
- **Deployment** adapts a role or orchestration pattern to a runtime and its available tools.
- **Conversation surface** is where a human interacts with the system, such as a local workspace or team chat.

The role specification must remain valid if any implementation, orchestrator, or conversation surface is replaced.

---

## Workflows

Workflows define repeatable processes.

Examples:

- validating an idea
- conducting market research
- launching a product
- reviewing quarterly performance
- retiring a project

Workflows evolve as experience grows.

---

## Templates

Templates reduce repetitive work while encouraging consistency.

Examples include:

- project proposals
- experiment plans
- customer interviews
- product specifications
- retrospective reviews
- decision records

Templates capture organisational knowledge.

---

## Portfolio

Rather than focusing on a single venture, Fibonacci OS manages a portfolio of activities.

A portfolio may contain:

- products
- services
- educational resources
- open-source projects
- research initiatives
- investments
- experiments

The portfolio is diversified intentionally.

---

# Information Flow

Information moves continuously throughout the operating system.

```text
Observation
      ↓
Research
      ↓
Evidence
      ↓
Decision
      ↓
Action
      ↓
Measurement
      ↓
Review
      ↓
Knowledge
      ↓
Improved Workflow
```

Every cycle increases organisational knowledge.

---

# Decision Flow

Decision-making remains human-centred.

```text
Human defines objective
        ↓
AI explores possibilities
        ↓
Evidence is collected
        ↓
Risks are evaluated
        ↓
Human makes decision
        ↓
AI assists implementation
        ↓
Results are reviewed
```

Responsibility always remains with humans.

---

# Modularity

Every component should be replaceable.

Examples:

- one AI model may be replaced by another
- one database may replace another
- one workflow may supersede another
- one project may be archived without affecting the rest of the system

Loose coupling encourages long-term sustainability.

---

# Local-First Design

The architecture prefers systems that:

- function offline when practical
- use open file formats
- preserve user ownership
- minimise vendor lock-in
- remain portable across platforms

Cloud services may enhance the operating system but should not become mandatory dependencies unless they provide clear and justified value.

---

# Relationship Between Documents

The documentation forms a coherent hierarchy.

```text
Philosophy
      ↓
Constitution
      ↓
Vision
      ↓
Architecture
      ↓
Workspace
      ↓
Agents
      ↓
Workflows
      ↓
Projects
```

Each document answers a different question:

- **Philosophy** — Why do we exist?
- **Constitution** — What principles guide us?
- **Vision** — Where are we going?
- **Architecture** — How is the system organised?
- **Workspace** — Where does work live?
- **Agents** — Who performs specialised roles?
- **Workflows** — How is work carried out?

Together they describe the operating system independently of any implementation.

---

# Evolution

The architecture is intentionally stable but not static.

As technologies, communities, and entrepreneurial practices evolve, the implementation may change significantly while preserving the underlying principles described in the Philosophy, Constitution, and Vision.

A successful architectural change makes Fibonacci OS simpler, more adaptable, and more effective without compromising its core values.
