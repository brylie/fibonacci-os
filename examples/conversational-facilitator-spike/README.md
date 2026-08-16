# Technical Spike: Conversational Facilitator Prototype

**Type:** Technical spike plan  
**Status:** Planned  
**Authoring date:** 2026-07-27  
**Trial start:** 2026-07-27  
**Trial end:** 2026-08-03  
**Owner:** Human project steward  
**Review date:** 2026-08-04 (after the one-week trial)

The parallel runtime comparison is documented in
[`parallel-comparison-plan.md`](parallel-comparison-plan.md).

## Purpose

Test whether a configured Facilitator agent within ChatGPT Work (referred to as
a Workspace Agent) can practically perform the Fibonacci Facilitator role during
real day-to-day work.

This is a learning exercise, not a production implementation. The outcome may
confirm, refine, or challenge the current architecture—or show that ChatGPT
Work is not the appropriate runtime.

Evidence is more valuable than confirmation.

## Objectives

The prototype should prioritise:

- simplicity
- manual operation
- architectural learning
- human oversight
- documentation-first workflows

Avoid unnecessary automation.

## Questions to Answer

### Workflow

- Can a single Workspace Agent successfully perform the Facilitator role?
- Does conversation naturally follow Fibonacci OS workflows?
- Where does conversation drift from the intended architecture?
- When should the Facilitator ask questions rather than make assumptions?
- How much information must remain visible to the human?

### Artefacts

- Can the agent reliably produce canonical Markdown artefacts?
- Which artefacts naturally emerge during conversation?
- Which artefacts feel artificial or create friction?
- Which useful artefacts are missing?

### Role Boundaries

- Can the Facilitator coordinate without becoming another specialist?
- Does it distinguish Recommendations from Requested Decisions?
- Does it preserve disagreement and uncertainty?
- Does it attribute substantive findings to source artefacts?

### User Experience

- Does interacting with the Facilitator feel natural?
- Does the architecture become unobtrusive during normal use?
- Which parts create unnecessary friction?
- Which parts reduce cognitive load?

### Workspace Capabilities

Investigate how these capabilities might support the Facilitator:

- instructions
- knowledge files
- conversation memory
- tools
- skills
- scheduled tasks
- integrations

Document capabilities without assuming they should all be used.

## Scope and Constraints

Use one Workspace Agent and manual operation only.

Do not build:

- automation pipelines
- orchestration engines
- multiple Workspace Agents
- APIs
- MCP servers
- databases
- vector search
- custom memory systems
- deployment scripts

The trial should use genuine work with sensitive information redacted or
excluded.

If one model performs multiple specialist perspectives, the result must be
described as a multi-role analysis rather than independent review.

## Prototype Shape

```text
Human objective
        ↓
Workspace Facilitator
        ↓
Clarifying questions
        ↓
Relevant specialist perspectives
        ↓
Canonical artefacts
        ↓
Coordination View
        ↓
Human decision
        ↓
Decision Record
        ↓
Experiment Plan or next action
        ↓
Lesson Learned
```

The exact workflow may change if evidence suggests a better approach. The
Facilitator must not make the human decision.

## Preparation

Provide the Workspace Agent with the smallest useful knowledge set:

- `docs/philosophy.md`
- `docs/constitution.md`
- `docs/architecture.md`
- `docs/artefacts.md`
- `docs/workflows.md`
- `agents/README.md`
- `agents/facilitator/README.md`
- `agents/facilitator/instructions.md`
- relevant specialist role specifications

Record which instructions, knowledge files, tools, integrations, and memory
features are actually enabled. Do not assume that a Workspace capability behaves
like a persistent memory system, orchestration engine, or independent agent
network.

## One-Week Trial

Run the Facilitator during genuine work for approximately one week. Suggested
activities include:

- evaluating an opportunity
- planning a project
- reviewing a decision
- organising research
- prioritising portfolio work
- reflecting on a completed experiment

Select three to five realistic, low-risk activities rather than creating
artificial demonstrations. Do not force every activity through the full
lifecycle. Observe whether the appropriate artefacts emerge naturally.

## Session Protocol

For each session, record:

1. Human objective
2. Initial context provided
3. Questions asked by the Facilitator
4. Artefacts produced
5. Specialist perspectives invoked
6. Recommendations and Requested Decisions
7. Disagreements or uncertainty preserved
8. Human corrections or interventions
9. Friction and useful moments
10. Final outcome

The human remains responsible for accepting, revising, or discarding artefacts
and for making consequential decisions.

## Observation Log

Create one observation for each meaningful finding:

```markdown
## Observation

**Date:**  
**Activity:**  
**Observation:**  
**Pain Point:**  
**Evidence:**  
**Severity:** Low | Medium | High  
**Architecture Change Needed?:** Yes | No | Unsure  
**Related Documents:**  
**Notes:**
```

Add a session identifier and links to resulting artefacts where useful. Record
observations before proposing architecture changes.

## Success Criteria

The spike succeeds if it increases understanding of how Fibonacci OS behaves in
real conversations—not because the Workspace Agent always follows the design
perfectly.

Evaluate whether the Facilitator can:

- begin with an ambiguous real objective
- ask useful clarifying questions
- select an appropriate workflow
- produce canonical artefacts without excessive friction
- coordinate specialist perspectives without becoming an unmarked analyst
- preserve disagreement and uncertainty
- distinguish Recommendations from Requested Decisions
- make human approval points visible
- support natural conversation while retaining durable knowledge
- avoid unnecessary artefacts and ceremony

## End-of-Week Review

Prepare a review covering:

1. Architectural assumptions that held
2. Assumptions that failed
3. Assumptions that remain untested
4. Natural conversations
5. Over-structured conversations
6. Useful artefacts
7. Ignored or artificial artefacts
8. Role-boundary failures
9. Facilitator coordination quality
10. Workspace capabilities that were actually useful
11. Documentation changes supported by evidence
12. Documentation that should remain unchanged
13. ChatGPT Workspace suitability
14. Recommended next experiment

Use three possible outcomes:

- continue with the current model
- continue with targeted refinements
- stop or change runtime

## Risks and Mitigations

- **Simulated independence:** label multi-role analysis honestly.
- **Unsupported factual claims:** require sources or mark external validation as
  pending.
- **Artificial task selection:** use genuine varied work.
- **Excessive structure:** record friction and ignored artefacts.
- **Unverified memory assumptions:** document observed Workspace behaviour.
- **Sensitive information exposure:** redact or exclude sensitive material.
- **Short-trial bias:** treat conclusions as provisional.

## Working Principles

- Architecture follows evidence.
- Simplicity comes before automation.
- Humans remain responsible for consequential decisions.
- Implementation independence must be preserved.
- Observations come before redesign.
- Many small improvements are preferred to one large redesign.

Treat Fibonacci OS itself as the subject of continuous learning. The goal is not
to build the final system, but to help Fibonacci OS learn about itself.
