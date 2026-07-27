# Glossary

> *This glossary defines the common language of Fibonacci OS. Shared terminology reduces ambiguity and enables consistent communication between humans, AI agents, and documentation.*

## Agent

A specialised operating-system role with clearly defined responsibilities, inputs, outputs, jurisdiction, and limitations. A role may be implemented by a human, AI system, deterministic software, workflow, or combination of these. Agents assist humans but do not possess decision-making authority.

---

## Artefact

A human-readable document exchanged between roles or workflow stages. An artefact records a question, evidence, reasoning, uncertainty, recommendation, or decision in a form that can be reviewed, preserved, and reused.

---

## Deployment

The adaptation of a canonical role or workflow for a particular runtime, tool set, knowledge source, approval model, or conversation surface. A deployment must not redefine the canonical role.

---

## Facilitator

The role that coordinates relevant specialist roles, preserves context, surfaces disagreement, synthesises findings, and returns consequential decisions to a human.

---

## Coordination View

A Facilitator-produced view that assembles references to source artefacts, convergence, disagreement, missing evidence, decisions required, and proposed next steps for a particular decision interaction. It is not currently a canonical artefact type and must not add independent specialist conclusions.

---

## Jurisdiction

The explicit boundary of what a role may observe, analyse, recommend, modify, or escalate. Jurisdiction prevents a role from acquiring authority merely because it can produce an output.

---

## Multi-role analysis

An analysis in which one implementation performs two or more role perspectives. It must not be represented as independent review unless independent roles or systems actually participated.

---

## Orchestration

The coordination of roles, workflow stages, context, handoffs, and human approval points. Orchestration is an implementation concern separate from the canonical role definitions.

---

## Runtime

The environment in which a role or workflow is carried out, such as a human process, language model, local application, deterministic service, or team-chat system.

---

## Archive

The collection of completed, retired, or superseded work that is preserved for historical reference and future learning.

---

## Architecture

The conceptual organisation of Fibonacci OS, describing how its principles, components, and workflows fit together independently of any implementation.

---

## Assumption

A statement believed to be true but not yet supported by sufficient evidence. Assumptions should be identified explicitly and validated where practical.

---

## Constitution

The enduring principles that govern Fibonacci OS. The Constitution takes precedence over implementation decisions, workflows, and technologies.

---

## Decision Record

A documented explanation of an important decision, including its rationale, supporting evidence, alternatives considered, and expected consequences.

---

## Recommendation

Advice owned by the role that produces an artefact, based on that role's analysis, evidence, assumptions, jurisdiction, and uncertainty. A recommendation is not a human decision.

---

## Requested Decision

A choice identified by an artefact for an authorised human to make. A requested decision remains unresolved until the responsible human confirms it.

---

## Evidence

Information that supports or challenges a claim. Evidence may include research, measurements, observations, experiments, financial data, or user feedback.

---

## Experiment

A small, intentional activity designed to reduce uncertainty by testing one or more assumptions.

Success is measured by learning rather than commercial outcome.

---

## Knowledge

Reusable understanding generated through experience, research, or reflection. Knowledge is considered one of the operating system's most valuable assets.

---

## Local-First

A design philosophy that prioritises user ownership by allowing work to be created, stored, and managed locally while remaining compatible with optional cloud services.

---

## Opportunity

A potential problem worth solving or a situation where meaningful value could be created.

Opportunities require validation before becoming projects.

---

## Philosophy

The statement of purpose that explains why Fibonacci OS exists and the values that motivate its development.

---

## Portfolio

The collection of projects, products, services, investments, and other assets managed within Fibonacci OS.

The portfolio is evaluated as a whole rather than as isolated initiatives.

---

## Product

A solution delivered to users that creates measurable value.

Products may include software, educational material, consulting services, physical goods, or digital resources.

---

## Project

A temporary initiative undertaken to investigate an opportunity, build a product, conduct research, or achieve another defined objective.

Projects have a beginning, an end, and a documented outcome.

---

## Research

The systematic collection of information used to improve understanding before making decisions.

Research supports evidence-based entrepreneurship.

---

## Review

A structured reflection on completed work intended to identify successes, shortcomings, lessons learned, and opportunities for improvement.

---

## Steward

An individual or AI agent responsible for protecting the long-term health of a particular aspect of the operating system, such as ethics, knowledge, or the portfolio.

Stewards guide and advise rather than control.

---

## Template

A reusable document or structure that captures proven practice and promotes consistency across projects.

---

## Validation

The process of testing assumptions with evidence before committing significant resources.

Validation reduces uncertainty and improves decision quality.

---

## Value

A positive outcome created for individuals, organisations, or communities.

Financial return is one form of value, but Fibonacci OS recognises educational, social, environmental, and personal value as equally important.

---

## Venture

An organised effort to create sustainable value.

A venture may consist of one or many related projects and products.

---

## Vision

The long-term aspiration describing what Fibonacci OS seeks to become and the impact it aims to have over time.

---

## Workflow

A repeatable sequence of activities that transforms inputs into meaningful outcomes.

Workflows capture organisational knowledge and provide a consistent framework for collaboration between humans and AI agents.

---

## Workspace

The organised environment in which projects, documentation, workflows, knowledge, and operational assets are stored and managed.

The workspace provides the shared structure that enables both humans and AI agents to work effectively.

---

# Terminology

When introducing new concepts, contributors should:

- reuse existing terms whenever possible
- define new terms before using them
- avoid creating synonyms for established concepts
- prefer clear, descriptive language over jargon

A shared vocabulary is essential to a shared operating system.
