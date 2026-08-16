# Parallel UX Comparison: ChatGPT Work and Claude Cowork

**Type:** Comparative technical spike plan  
**Status:** Planned  
**Date:** 2026-07-27  
**Related spike:** [Conversational Facilitator Prototype](README.md)  
**Review date:** After the paired trial

## Purpose

Compare the user experience of running the same Fibonacci Facilitator prototype
in ChatGPT Work and Claude Cowork, including work that begins or continues on a
mobile phone away from the laptop.

This is a runtime comparison, not a product benchmark or a test of which model
is more capable in general. The core question is whether either environment
helps a human use the Facilitator role naturally while preserving artefacts,
uncertainty, role boundaries, and human authority.

## Current Product Context

The official product documentation describes the following capabilities:

- [ChatGPT Work](https://openai.com/chatgpt-work/) is described as available on
  macOS and Windows desktop, and on web and mobile for specified paid and
  education plans. The page describes working with tools and files, checking
  progress from a phone, tasks, and plan review.
- [Claude Cowork](https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork)
  is described as available on desktop, web, and mobile for paid plans, with
  remote sessions that can be continued across surfaces. The documentation also
  describes project context, approval modes, local-file access through desktop,
  and remote work that can continue while the user is away.

These are documented capabilities, not observations from this trial.
Availability, rollout, plan limits, and actual behaviour must be recorded
separately.

## Comparison Principles

- Use the same Facilitator role definition and behavioural instructions in both
  environments.
- Provide the same knowledge pack and task context where the products allow.
- Keep the core comparison limited to conversation, artefacts, and human
  decision support.
- Compare native features separately rather than penalising one runtime for not
  matching another's product design.
- Distinguish documented capability, observed behaviour, and user impression.
- Run paired tasks close enough in time that the underlying work context remains
  comparable.
- Do not use sensitive personal, financial, legal, or confidential information.
- Keep consequential actions, publication, spending, and external communication
  under explicit human control.

## Prototype Configuration

Use one Facilitator workspace or project in each environment. Do not add
multiple agents, orchestration, bots, APIs, or custom memory systems.

Provide the same minimum knowledge pack:

- `docs/philosophy.md`
- `docs/constitution.md`
- `docs/architecture.md`
- `docs/artefacts.md`
- `docs/workflows.md`
- `agents/README.md`
- `agents/facilitator/README.md`
- `agents/facilitator/instructions.md`
- relevant specialist role specifications

If a platform cannot access the repository directly, upload the same files or an
identical prepared bundle. Record any differences in setup effort, file
handling, context limits, and persistence.

## Local Workspace Separation

Runtime-specific working files belong in the ignored local directories:

```text
workspace/
├── chatgpt/
└── claude/
```

Use `workspace/chatgpt/` for ChatGPT Work prompts, exports, transcripts, drafts,
and temporary files. Use `workspace/claude/` for Claude Cowork equivalents. Keep
the comparison plan, canonical documentation, and reviewed observations outside
these directories so they remain shareable and version-controlled.

## Core Task Suite

Use the same tasks in both environments. Prefer genuine work; the following
sequence provides a repeatable minimum:

### Task A: Opportunity framing

Use the Finland immigrant-services directory opportunity from the existing
prototype. Ask the Facilitator to clarify the objective and produce an
Opportunity Brief without claiming external research.

Observe clarification quality, evidence discipline, and whether the conversation
feels natural.

### Task B: Decision support

Continue from Task A or provide the same Opportunity Brief. Ask for explicit
specialist perspectives and a Coordination View. Require the Facilitator to
preserve disagreement and leave the Requested Decision unresolved.

Observe role boundaries, artefact fidelity, attribution, and human control.

### Task C: Mobile interruption and continuation

Start a task on the laptop, leave it at a natural pause, and continue from the
phone. Then perform the reverse direction if practical.

On mobile, ask the Facilitator to:

- summarise the current state
- ask one clarifying question
- steer the next step
- review or correct a short artefact section

Observe context continuity, reading and editing friction, notification or status
usefulness, and whether the phone is a viable control surface.

### Task D: Real work variation

Use one additional genuine activity such as project planning, research
organisation, portfolio prioritisation, or decision review. Keep the task and
supplied context identical across environments where possible.

Observe whether the runtime remains useful outside the reference opportunity.

## Comparison Conditions

Run at least these conditions when supported:

| Condition                     | Laptop             | Mobile             | Purpose                                                      |
| ----------------------------- | ------------------ | ------------------ | ------------------------------------------------------------ |
| Foreground conversation       | Start and continue | Not applicable     | Baseline Facilitator UX                                      |
| Laptop-to-mobile continuation | Start              | Continue           | Context handoff and mobile control                           |
| Mobile-to-laptop continuation | Continue on laptop | Start              | Whether mobile input can initiate useful work                |
| Away-from-device task         | Start              | Check and steer    | Whether asynchronous work is understandable and controllable |

If a condition is unavailable in one environment, record it as unavailable
rather than treating it as a failure of the Facilitator architecture.

## Mobile UX Questions

Record observations about:

- ease of starting a task from the phone
- ability to supply context without a laptop file browser
- readability of long artefacts
- ease of correcting or approving a step
- ability to answer clarifying questions quickly
- visibility into what the system is doing
- interruption and resume behaviour
- notification usefulness and noise
- confidence that the correct project or session is open
- whether mobile is suitable for steering, reviewing, or only monitoring

Do not assume mobile should support full authoring. Determine which activities
are genuinely comfortable and useful.

## UX Measures

Use short qualitative notes first. Optional Low / Medium / High ratings may be
added after the session for:

- setup effort
- time to first useful response
- clarification quality
- artefact usefulness
- context continuity
- mobile effort
- perceived control
- confidence in decision boundaries
- recovery after interruption
- output portability

Also record a concrete example for every rating that differs between
environments.

## Observation Record

```markdown
## Observation

**Session ID:**  
**Runtime:** ChatGPT Work | Claude Cowork  
**Surface:** Laptop | Mobile | Handoff  
**Task:**  
**Condition:**  
**Date:**  
**Documented capability or observed behaviour:**  
**Observation:**  
**Pain Point:**  
**Evidence:**  
**Severity:** Low | Medium | High  
**Architecture Change Needed?:** Yes | No | Unsure  
**Related Artefacts:**  
**Notes:**
```

Use one record for a meaningful observation, not one record for every message.

## Evidence Discipline

For every comparison claim, label it as one of:

- **Documented** — stated in an official product source.
- **Observed** — directly experienced during the paired trial.
- **Inferred** — an interpretation of observed behaviour.
- **Unresolved** — not tested or not reproducible.

Do not treat a smoother or slower session as evidence of architectural
superiority without recording the task, setup, surface, and actual interaction.

## Safety and Control Boundaries

- Use manual approval for consequential actions.
- Do not connect personal accounts or sensitive folders for the first
  comparison.
- Do not enable scheduled tasks, browser actions, external messaging, or
  write-capable integrations unless the comparison specifically requires them
  and the human approves.
- Record whether a task runs remotely, locally, or through a desktop bridge.
- If one environment continues work while the user is away, compare the
  visibility and control of that behaviour rather than treating unattended
  execution as automatically better.
- Label any single-model multi-role analysis honestly.

## Paired Review Questions

After both environments complete the same task, compare:

1. Which environment required less setup?
2. Which asked better clarifying questions?
3. Which made the workflow feel more natural?
4. Which produced more useful and portable artefacts?
5. Which better preserved Recommendations, Requested Decisions, and unresolved
   disagreement?
6. Which gave the human better visibility and control?
7. Which handled interruption and mobile continuation better?
8. Which capabilities were genuinely useful rather than merely available?
9. Where did either environment encourage overreach, hidden assumptions, or
   premature action?
10. Which differences are runtime UX differences, and which reveal limitations
    in the Facilitator architecture?

## Decision Rule

Do not choose a runtime based on a single impressive output. At the end of the
trial, choose one of:

- **Continue with one runtime** for the next Facilitator experiment.
- **Continue with both** because they serve different working conditions.
- **Refine the shared Facilitator configuration** before choosing.
- **Stop using either as the primary prototype runtime** because the UX or
  control model is unsuitable.

The decision must remain separate from the product vendors' own feature claims.

## Expected Deliverables

- paired task notes
- observation records
- saved Opportunity Brief and Coordination View from both environments where
  practical
- mobile continuation notes
- end-of-trial comparison review
- unresolved questions and recommended next experiment

Do not change the canonical role or artefact specifications during the
comparison unless repeated observations provide clear evidence. Record
speculative improvements separately.
