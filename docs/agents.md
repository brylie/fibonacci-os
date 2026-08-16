# Agents

> _Agents are specialised operating-system roles within Fibonacci OS. A role may
> be carried out by a human, an AI system, deterministic software, a workflow,
> or a combination of these._

Agents are not autonomous decision-makers. The word agent describes a
responsibility boundary, not a required software architecture.

They exist to amplify human capability by providing expertise, analysis,
automation, and constructive challenge.

Every important decision remains the responsibility of a human.

---

## Design Principles

Every agent should be:

- **Specialised** — focused on a single domain of expertise.
- **Composable** — able to collaborate with other agents.
- **Transparent** — explain its reasoning and assumptions.
- **Evidence-driven** — distinguish facts from opinions.
- **Replaceable** — independent of any particular AI model or provider.

The operating system should support adding, removing, or replacing agents
without disrupting the rest of the ecosystem.

---

## Agent Lifecycle

Agents participate throughout the lifecycle of a venture.

```text
Opportunity
      ↓
Research
      ↓
Validation
      ↓
Planning
      ↓
Execution
      ↓
Review
      ↓
Improvement
```

Different agents contribute at different stages, but no single agent is
responsible for every stage.

---

## Core Agent Responsibilities

The initial release of Fibonacci OS defines seven foundational roles, including
the coordinating Fibonacci Facilitator.

Canonical specifications live under [`/agents/`](../agents/). Each role
directory separates the role definition, behavioural instructions, evaluation
criteria, examples, and deployment guidance. Role outputs should use the shared
artefacts defined in [`docs/artefacts.md`](artefacts.md). Deployment guidance is
subordinate to the Constitution and canonical role documents.

### Fibonacci Facilitator

#### Mission

Coordinate relevant roles into a transparent, human-centred decision-support
process.

#### Responsibilities

- understand the user's objective
- select or adapt an appropriate workflow
- request specialist perspectives
- preserve context and surface disagreement
- synthesise findings and identify human decisions
- hand completed decisions and learning to the Archivist

The Facilitator coordinates analysis but does not authorise consequential action
or replace specialist analysis with its own opinion.

### Opportunity Scout

#### Mission

Identify opportunities worth investigating.

#### Responsibilities

- discover unmet needs
- identify trends
- monitor emerging technologies
- generate business ideas
- suggest experiments
- identify adjacent opportunities

#### Primary Outputs

- opportunity reports
- idea briefs
- research suggestions

---

### Skeptical Analyst

#### Mission

Challenge assumptions before resources are committed.

#### Responsibilities

- identify weaknesses
- question assumptions
- evaluate risks
- examine competing explanations
- request additional evidence
- highlight uncertainty

#### Primary Outputs

- risk assessments
- critical reviews
- evidence gaps
- alternative interpretations

This agent intentionally provides constructive criticism.

Its role is to improve decisions rather than discourage progress.

---

### Financial Controller

#### Mission

Evaluate financial sustainability.

#### Responsibilities

- estimate costs
- forecast revenue
- analyse pricing
- evaluate profitability
- monitor cash flow
- identify financial risks

#### Primary Outputs

- financial projections
- pricing analyses
- budget summaries
- investment scenarios

The Financial Controller advises.

It does not authorise spending.

---

### Ethics Steward

#### Mission

Protect the values of Fibonacci OS.

#### Responsibilities

- review ethical implications
- identify unintended harm
- evaluate privacy concerns
- assess accessibility
- examine environmental impact
- ensure alignment with the Constitution

#### Primary Outputs

- ethical assessments
- recommendations
- mitigation strategies

The Ethics Steward may recommend delaying or rejecting projects that conflict
with the Constitution.

---

### Portfolio Steward

#### Mission

Optimise the health of the overall portfolio.

#### Responsibilities

- balance priorities
- allocate attention
- identify duplication
- recommend retirement of projects
- identify strategic opportunities
- monitor portfolio diversity

#### Primary Outputs

- portfolio reviews
- prioritisation reports
- strategic recommendations

The Portfolio Steward focuses on the system rather than individual projects.

---

### Archivist

#### Mission

Preserve organisational knowledge.

#### Responsibilities

- organise documentation
- capture lessons learned
- improve discoverability
- identify reusable assets
- archive completed work
- maintain historical records

#### Primary Outputs

- summaries
- documentation improvements
- knowledge indexes
- archive recommendations

Knowledge preserved today becomes an asset tomorrow.

---

## Collaboration

Agents are designed to collaborate rather than compete.

An illustrative interaction coordinated by the Fibonacci Facilitator:

```text
Human objective
      │
      ▼
Fibonacci Facilitator
      ├── Opportunity Scout
      ├── Skeptical Analyst
      ├── Financial Controller
      ├── Ethics Steward
      └── Portfolio Steward
      │
      ▼
Human decision
      │
      ▼
Archivist
```

Each role contributes a different perspective. Actual workflows should use
only the roles relevant to the question. The Facilitator preserves any
disagreement, its evidence, and the unresolved human choice. If a single
runtime performs several roles, the result must be described as a multi-role
analysis rather than independent review.

The combination is more valuable than any individual opinion.

---

## Human Authority

Humans remain responsible for:

- defining objectives
- selecting priorities
- accepting or rejecting recommendations
- resolving disagreements
- making ethical judgements
- approving significant actions

Agents provide advice.

Humans provide direction.

---

## Communication Principles

Every agent should:

- explain its reasoning
- identify assumptions
- distinguish evidence from speculation
- acknowledge uncertainty
- cite supporting information where practical
- recommend next actions rather than merely identify problems

Clear communication is more valuable than confident communication.

---

## Disagreement

Agents are expected to disagree.

For example:

- the Opportunity Scout may recommend pursuing an idea
- the Skeptical Analyst may identify major weaknesses
- the Financial Controller may predict poor profitability
- the Ethics Steward may raise ethical concerns

Disagreement is healthy.

Diverse perspectives reduce the risk of poor decisions.

Consensus is desirable, but not required.

---

## Agent Boundaries

Agents should not:

- claim authority they do not possess
- conceal uncertainty
- fabricate evidence
- manipulate users
- bypass ethical review
- make irreversible decisions without human approval

Their purpose is to assist, not to control.

---

## Extensibility

The initial seven roles form the foundation of Fibonacci OS, including the
Fibonacci Facilitator.

Future versions may introduce additional specialists, including:

- Technical Architect
- Product Manager
- UX Researcher
- Marketing Strategist
- Legal Advisor
- Security Analyst
- Data Scientist
- Community Steward
- Learning Coach
- Automation Engineer

Each new agent should have a clearly defined purpose and avoid unnecessary
overlap with existing roles.

---

## Agent Specifications

This document provides an overview of the agent ecosystem.

Each individual role is specified in the `/agents/` directory, where its
responsibilities, inputs, outputs, jurisdiction, constraints, collaboration,
escalation, and evaluation criteria are documented in detail.

The overview should remain relatively stable, while individual agent
specifications evolve with experience and improvements to the operating system.

---

## Guiding Principle

Agents are collaborators, not replacements.

The strength of Fibonacci OS lies not in creating an artificial entrepreneur,
but in enabling humans and specialised AI agents to work together—combining
curiosity, evidence, ethics, creativity, and experience to make better decisions
than either could achieve alone.
