# Deferred Ideas

This document records potentially useful ideas that are not currently approved
for implementation. Recording an idea does not place it on the roadmap or
authorize work.

## Document Retrieval Tooling

### Graphify

**Status:** Deferred

**Idea:** Build a queryable knowledge graph from code, documentation, papers,
and diagrams to help coding assistants navigate a larger repository.

**Why deferred:** The Conversational Facilitator trial is intentionally manual
and does not include custom retrieval, knowledge-graph, memory, or orchestration
systems. The current Markdown workspace is small enough for targeted reading and
search.

**Revisit when:** Repeated observations show that targeted reading and search
miss relevant context, create unreliable handoffs, or materially slow work.

### Docling

**Status:** Deferred

**Idea:** Convert complex and unstructured documents into structured,
AI-ready content.

**Why deferred:** No current task requires repeated document conversion, and
introducing a document-processing pipeline would exceed the scope of the manual
trial.

**Revisit when:** The project needs to use a recurring set of complex documents
that cannot be reliably reviewed in their original format, and a bounded
evaluation can establish clear value, privacy controls, and ownership of derived
data.

## Review Practice

Review deferred ideas during a roadmap or technical-spike discussion. Move an
idea into a proposed experiment only when there is a specific problem, evidence
that the current approach is insufficient, and an explicit human decision to
test it.
