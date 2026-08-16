# Provisional Lesson Learned: Architectural Walkthrough

**Type:** Lesson Learned  
**Status:** Provisional  
**Date:** 2026-07-27  
**Author or role:** Archivist, based on the completed walkthrough  
**Related project or opportunity:** Finland Immigrant Services Directory  
**Review date:** After human review of the prototype

## Context and Original Expectation

The prototype was intended to test whether implementation-independent roles and
Markdown artefacts could support a coherent manual workflow without runtime
code, exhaustive research, or an autonomous decision.

The expected result was a chain of specialist artefacts that preserved evidence
boundaries, disagreement, and human approval points.

## What Happened

The workflow produced an Opportunity Brief, Critical Review, Ethics Assessment,
Financial Assessment, Portfolio Assessment, Facilitator Synthesis, unresolved
Decision Record, minimal Experiment Plan, and this Lesson Learned.

The absence of external research did not prevent structural testing, but it
limited the strength of domain conclusions. The artefacts were able to mark that
limitation explicitly.

## Evidence

- Every role had a named output artefact.
- The specialist artefacts produced distinct concerns: intervention fit, safety,
  sustainability, and portfolio capacity.
- The Facilitator could assemble those concerns without claiming independent
  specialist analysis.
- The Decision Record could remain unresolved while still being useful.
- The Experiment Plan converted uncertainty into bounded questions rather than
  assuming product approval.

## What Was Learned

1. The shared artefact model gives role boundaries a practical interface: each
   role can answer a different question in a durable form.
2. Common metadata and repeated sections make artefacts understandable out of
   context, but they also create repetition.
3. The Facilitator needs an explicit prohibition against becoming an additional
   analyst; otherwise “synthesis” can easily become an unmarked opinion.
4. The Ethics Assessment materially changed the experiment boundary by
   challenging “authoritative,” personal-data collection, and public release.
5. The Financial Assessment was useful without numeric forecasts because it
   identified maintenance, stewardship, and recurring obligations as the main
   unknowns.
6. The Portfolio Assessment requires actual portfolio and capacity data to move
   beyond a principled recommendation.
7. The artefact chain supports a human decision without pretending that a
   workflow has made one.

## What Remains Uncertain

- whether the proposed user problem exists at meaningful scale
- whether a directory is better than other interventions
- what source and maintenance model is feasible
- how users interpret authority, attribution, and limitations
- whether the current artefact sections remain usable with real research
  evidence

## Implications for Projects, Workflows, or Roles

The next test should use the same artefact forms with real external sources and
a narrow user task. It should not introduce machine schemas or orchestration
until the Markdown handoffs have been exercised more than once.

The Facilitator specification should continue to distinguish coordination from
specialist analysis. The Archivist should preserve both the artefacts and their
evidence boundary.

## Reusable Assets

- the artefact contract in [`docs/artefacts.md`](../../docs/artefacts.md)
- this complete manual walkthrough
- the unresolved Decision Record pattern
- the bounded Experiment Plan pattern

## Recommended Changes

No canonical documentation change is required solely from this first
walkthrough. The main observations should be tested again before changing the
contract. Potential future improvements are recorded in the validation report
rather than applied speculatively.

## Confidence

Medium that the architecture is coherent enough for another manual prototype;
low that the artefact fields are final or that the opportunity itself is
validated.

## Related Decision or Experiment

- [`Draft Decision Record`](decision-record.md)
- [`Draft Experiment Plan`](experiment-plan.md)
