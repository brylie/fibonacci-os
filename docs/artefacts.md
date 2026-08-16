# Artefacts

> _Artefacts are the shared language of Fibonacci OS. They are human-readable
> documents exchanged between people, roles, workflows, and implementations._

## Purpose

Roles should exchange durable artefacts rather than rely on private or
unrecorded conversation. A canonical artefact makes the question, evidence,
uncertainty, recommendation, and required human judgement visible to every
participant.

These specifications are intentionally written in Markdown. They are not JSON
schemas, API contracts, or vendor configuration. Machine-readable formats may be
derived later if practical, but they must preserve the meaning and human
readability of these documents.

## General Principles

- An artefact records work; it does not grant authority.
- Evidence, assumptions, interpretation, and recommendation must remain
  distinguishable.
- A recommendation is not a decision until a human makes and records that
  decision.
- Artefacts should preserve provenance, uncertainty, dissent, and relevant
  privacy boundaries.
- A later summary may improve discoverability but must not silently rewrite
  history.
- Use only the artefacts needed for the workflow; do not create documents for
  ceremony.

## Common Metadata

Every artefact should begin with the information that makes it understandable
out of context:

```markdown
# [Artefact title]

**Type:** [canonical artefact type]
**Status:** Draft | Provisional | Active | Superseded | Archived
**Date:** [YYYY-MM-DD]
**Author or role:** [person, role, or implementation]
**Related project or opportunity:** [link or name]
**Review date:** [date, event trigger, or Not scheduled]
```

The body should identify the relevant question or purpose, evidence,
assumptions, risks or uncertainties, recommendation, confidence, and requested
decision or next action where applicable. `Review date` may be a calendar date
or a workflow trigger (such as `At human decision point` or `Before next experiment`).
A field may be marked `Not known` rather than invented.

## Recommendations and Human Decisions

**Recommendation** is owned by the role producing the artefact. It expresses
that role's analysis-based advice, subject to its evidence, assumptions,
jurisdiction, and uncertainty.

**Requested Decision** identifies a choice reserved for an authorised human. It
is not an output that the role may make on the human's behalf.

A recommendation must not be presented as though the requested decision has
already been made. When no human decision has occurred, the artefact should say
so explicitly.

## Artefact Relationships

```text
Opportunity Brief
        │
        ├── Critical Review
        ├── Ethics Assessment
        ├── Financial Assessment
        └── Portfolio Assessment
                │
                ▼
          Human decision
                │
        ├── Experiment Plan
        └── Decision Record
                │
                ▼
          Lesson Learned
```

This is a common pattern, not a mandatory sequence. A workflow may repeat, skip,
or combine stages while preserving the artefact meanings.

## Facilitator Synthesis as a Coordination View

The Facilitator Synthesis is currently a **coordination view**, not a ninth
canonical artefact type. It supports a particular decision interaction by
assembling references to source artefacts, convergence, disagreement, missing
evidence, decisions required, and proposed next steps.

A coordination view must attribute every substantive finding to the originating
specialist artefact. It must not introduce independent specialist conclusions or
make a human decision. It may be preserved when useful for context, but its
primary purpose is to support the interaction in which the Facilitator
coordinates the work.

## Canonical Artefacts

### Opportunity Brief

Frames a potential problem or opportunity before it is treated as validated.

Required sections:

- **Question or observation** — what was noticed and what needs understanding
- **Affected people or context** — who experiences the situation and when
- **Current alternatives** — how the need is handled today
- **Evidence** — observations, research, feedback, or measurements
- **Assumptions** — claims that still require testing
- **Risks and exclusions** — possible harm, bias, or missing perspectives
- **Opportunity hypothesis** — the value that might be created
- **Proposed investigation** — the smallest useful research or experiment
- **Confidence**
- **Requested next action** — normally a human decision to investigate

The Opportunity Scout commonly prepares this artefact. It must describe a
hypothesis, not claim validation.

### Critical Review

Tests whether a proposal or claim survives constructive examination.

Required sections:

- **Proposal under review**
- **Evidence examined**
- **Assumptions and dependencies**
- **Counterarguments or competing explanations**
- **Material risks and failure conditions**
- **Findings** — including strengths and weaknesses
- **Evidence needed next**
- **Recommendation**
- **Confidence**
- **Requested decision or test**

The Skeptical Analyst commonly prepares this artefact. It should improve
learning rather than block all action.

### Ethics Assessment

Examines whether proposed work respects people, communities, and the
Constitution.

Required sections:

- **Proposal and scope**
- **Affected parties** — including people who may be excluded or indirectly
  affected
- **Potential benefits and harms**
- **Privacy, consent, and autonomy**
- **Fairness, accessibility, and power**
- **Environmental considerations**
- **Evidence and uncertainty**
- **Mitigations and safeguards**
- **Residual risk**
- **Recommendation or escalation**
- **Confidence**
- **Human approval required**

The Ethics Steward commonly prepares this artefact. A mitigation does not
automatically eliminate residual risk.

### Financial Assessment

Explains the financial implications and sustainability of a proposal or
experiment.

Required sections:

- **Scope, period, and currency**
- **Inputs and assumptions**
- **Costs and resource needs**
- **Revenue, pricing, or savings logic where relevant**
- **Cash implications**
- **Scenarios** — such as base, downside, and upside where useful
- **Sensitivity and material financial risks**
- **Non-financial value not represented by the model**
- **Recommendation**
- **Confidence**
- **Human approval required**

The Financial Controller commonly prepares this artefact. Estimates must show
their assumptions and must not authorise spending.

### Portfolio Assessment

Explains how work fits within the wider portfolio and available capacity.

Required sections:

- **Portfolio question**
- **Relevant projects, assets, and objectives**
- **Capacity and dependencies**
- **Strategic fit and duplication**
- **Opportunity cost and concentration risk**
- **Value, learning, and sustainability considerations**
- **Options and consequences**
- **Recommendation**
- **Confidence**
- **Requested human decision**

The Portfolio Steward commonly prepares this artefact. It may recommend pausing
or retiring work but cannot do so itself.

### Decision Record

Preserves a consequential human decision and its rationale.

Required sections:

- **Decision requested**
- **Decision made** — explicitly recorded as a human decision
- **Decision owner and date**
- **Context**
- **Options considered**
- **Evidence and assumptions**
- **Role contributions and disagreements**
- **Rationale**
- **Consequences and commitments**
- **Review trigger or date**
- **Related artefacts**

The Facilitator may prepare a draft, but the decision must not be presented as
made until the responsible human confirms it. The Archivist commonly preserves
the final record.

### Experiment Plan

Defines a bounded activity intended to reduce uncertainty.

Required sections:

- **Question**
- **Hypothesis**
- **Intervention or method**
- **Participants or data**
- **Measures and observations**
- **Learning criteria** — what would support, weaken, or change the hypothesis
- **Resources and timebox**
- **Ethical safeguards**
- **Stop or escalation conditions**
- **Owner**
- **Requested approval**

An experiment plan should be proportionate to the uncertainty and must not imply
that learning guarantees commercial success.

### Lesson Learned

Captures reusable understanding from an experiment, project, or decision.

Required sections:

- **Context and original expectation**
- **What happened**
- **Evidence**
- **What was learned**
- **What remains uncertain**
- **Implications for projects, workflows, or roles**
- **Reusable assets**
- **Recommended changes**
- **Confidence**
- **Related decision or experiment**

The Archivist commonly prepares this artefact from human-approved source
material. It should preserve surprising or negative results rather than only
successful stories.

## Artefact Handoffs

When handing an artefact to another role, identify:

- what question the recipient should answer
- which sections are authoritative source material
- which assumptions require review
- what output artefact is requested
- what human approval boundary applies

The receiving role should return an artefact of the requested type or clearly
explain why another type is more appropriate. Informal conversation may support
the work, but the durable handoff is the artefact.

## Status and History

Artefacts may move from `Draft` to `Active`, then become `Superseded` or
`Archived`. Superseded artefacts remain available when they explain historical
reasoning. Corrections should preserve the original record and identify the
correction rather than silently changing a material conclusion.

## Privacy and Ownership

Artefacts should contain only the information needed for their purpose.
Personal, financial, confidential, or commercially sensitive material must
follow the workspace's privacy rules. Users retain ownership of their artefacts
and should be able to move, inspect, edit, and archive them using portable text
formats.

## Future Derivations

Once these forms have been exercised manually, the project may derive
machine-readable representations such as JSON Schema or YAML. Such
representations are implementation aids, not replacements for these
human-readable specifications.
