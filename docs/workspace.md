# Workspace

> *The workspace is the home of Fibonacci OS. It provides a consistent structure for organising knowledge, projects, AI collaboration, and operational assets.*

The workspace is designed to answer a simple question:

> **"If I return to this project in five years, will I immediately understand where everything lives?"**

A predictable structure reduces cognitive load, makes automation easier, and enables both humans and AI agents to navigate the operating system consistently.

---

# Design Principles

The workspace should be:

- **Human-readable** — understandable without specialised software.
- **AI-friendly** — organised so agents can reliably discover and process information.
- **Local-first** — fully functional on a local computer.
- **Portable** — independent of any cloud provider or vendor.
- **Modular** — capable of supporting one project or hundreds.
- **Version-controlled** — text-based artefacts should work naturally with Git.

---

# Workspace Structure

```text
workspace/
│
├── inbox/
├── projects/
├── portfolio/
├── research/
├── workflows/
├── templates/
├── agents/
├── finance/
├── reviews/
├── decisions/
├── knowledge/
├── archive/
└── system/
```

Each directory has a distinct responsibility.

---

# inbox/

The inbox is a temporary holding area.

Examples include:

- ideas
- notes
- bookmarks
- voice transcriptions
- meeting notes
- screenshots
- links

Nothing should remain in the inbox permanently.

Items should eventually be:

- organised
- converted into projects
- archived
- discarded

---

# projects/

Projects are active initiatives.

Each project has its own directory.

Example:

```text
projects/
    piano-course/
    local-marketplace/
    fibonacci-income/
```

A project may contain:

- documentation
- source code
- assets
- experiments
- marketing
- financial notes
- reviews

Projects have a lifecycle.

When complete, they are archived rather than deleted.

---

# portfolio/

The portfolio provides a high-level view of everything being managed.

It records information such as:

- active ventures
- recurring income
- investments
- open-source projects
- educational products
- consulting work

The portfolio answers:

> What do we own?
>
> What creates value?
>
> Where should attention be focused?

---

# research/

Research contains information gathered before making decisions.

Examples include:

- market analysis
- customer interviews
- competitor research
- academic papers
- industry reports
- technical investigations

Research supports evidence-based decision-making.

---

# workflows/

Reusable operating procedures.

Examples include:

- validating an idea
- conducting interviews
- launching a product
- publishing documentation
- quarterly reviews

Workflows evolve continuously as experience grows.

---

# templates/

Templates eliminate repetitive work.

Examples include:

- project proposal
- experiment plan
- meeting agenda
- product specification
- retrospective
- decision record

Templates represent accumulated organisational knowledge.

---

# agents/

The agents directory contains AI role definitions.

Examples include:

- Opportunity Scout
- Portfolio Steward
- Skeptical Analyst
- Financial Controller
- Ethics Steward
- Archivist

Each agent has:

- responsibilities
- inputs
- outputs
- constraints
- success criteria

Agents should remain independent and composable.

---

# finance/

Financial information is organised separately from projects.

Examples include:

- budgets
- revenue
- expenses
- invoices
- subscriptions
- tax records
- forecasts

Sensitive financial information should remain private.

Only aggregated or intentionally shared information should become public.

---

# reviews/

Reviews capture reflection.

Examples include:

- weekly reviews
- monthly reviews
- quarterly reviews
- annual reviews
- project retrospectives

The purpose is continuous improvement rather than judgement.

---

# decisions/

Important decisions should be recorded.

Each decision record should answer:

- What was decided?
- Why?
- What evidence supported it?
- What alternatives were considered?
- Who made the decision?
- When should it be reviewed?

Decision records preserve organisational memory.

---

# knowledge/

Knowledge contains reusable information produced by the operating system.

Examples include:

- lessons learned
- best practices
- technical notes
- design patterns
- educational material
- reusable prompts
- implementation guides

Knowledge should outlive individual projects.

---

# archive/

Completed work belongs here.

Examples include:

- retired projects
- obsolete experiments
- superseded workflows
- historical documentation

Nothing should be deleted simply because it is no longer active.

Archived knowledge often becomes valuable again.

---

# system/

The system directory contains the operating system itself.

Examples include:

- documentation
- configuration
- schemas
- automation
- scripts
- governance
- operating principles

This directory defines how Fibonacci OS operates independently of the user's projects.

---

# Project Structure

Each project should follow a consistent structure.

```text
project/
│
├── README.md
├── notes/
├── research/
├── experiments/
├── product/
├── marketing/
├── finance/
├── reviews/
├── assets/
└── archive/
```

Projects may extend this structure as needed while preserving its overall organisation.

---

# Public and Private Information

The workspace intentionally separates public and private information.

Public examples:

- documentation
- open-source code
- templates
- educational resources

Private examples:

- financial records
- customer information
- credentials
- contracts
- unpublished strategy

Sensitive information should never be committed to public repositories.

---

# AI Collaboration

AI agents should treat the workspace as a shared environment.

Agents may:

- read documentation
- generate drafts
- analyse information
- suggest improvements
- automate repetitive tasks

Agents should not:

- overwrite important information without review
- modify financial records autonomously
- make irreversible decisions
- access sensitive information beyond their responsibilities

The workspace is collaborative.

It is never autonomous.

---

# Naming Conventions

Consistency is more valuable than perfection.

Recommended conventions:

- lowercase directory names
- kebab-case for files and folders
- ISO 8601 dates (`YYYY-MM-DD`)
- Markdown for documentation
- UTF-8 text encoding

Predictable naming simplifies both navigation and automation.

---

# Evolution

The workspace is designed to evolve.

New directories, workflows, and tools may be added as Fibonacci OS grows, but changes should preserve the core principles of clarity, consistency, portability, and user ownership.

A well-organised workspace enables every project to contribute not only to its own success, but to the continual improvement of the operating system itself.
