# Product Engineering Operating System (PEOS)

> **Build better products by making better decisions before writing code.**

PEOS is an opinionated operating system for AI-assisted product development.

It provides a repeatable workflow for building software products where humans remain responsible for decisions while AI agents accelerate execution.

PEOS is technology-agnostic.

It is not tied to Swift, React, Node.js, OpenAI, Claude, or any specific implementation.

Instead, it defines **how teams think, decide and collaborate** when building products with AI.

---

# Philosophy

PEOS is based on one simple principle:

> **Humans own decisions. AI owns execution.**

AI agents are encouraged to:

- propose
- analyse
- implement
- review
- test
- document

Humans remain responsible for:

- product vision
- technical strategy
- architecture
- approvals

Implementation is the consequence of approved decisions—not the place where those decisions are discovered.

---

# Core Principles

Every PEOS project follows the same immutable principles.

These principles define how work flows across the system and who owns each decision.

Start here:

- `docs/core-principles.md`

---

# Reading Order

New contributors and AI agents should read the documentation in the following order:

1. Core Principles
2. Development Flow
3. Development Horizons
4. Decision Authority
5. Roles
6. Project Adoption
7. Templates

Following this order ensures a shared understanding of both the philosophy and the workflow before implementation begins.

---

# Development Process

PEOS organizes software development into clearly defined stages.

Each stage has explicit owners, responsibilities and deliverables.

Typical flow:

```text
Idea
    ↓
Product Roadmap
    ↓
Epic Specification
    ↓
Technical Strategy
    ↓
Implementation Proposal
    ↓
Approval
    ↓
Delivery
    ↓
Epic Acceptance
    ↓
Merge
    ↓
Documentation Update
```

See:

- `docs/development-flow.md`
- `docs/development-horizons.md`
- `docs/decision-authority.md`

---

# Repository Structure

```
docs/
    Core principles
    Development process
    Roles
    Adoption guides

templates/
    Reusable documentation templates

.cursor/
    Agents
    Skills
    Rules

bootstrap/
    Prompts for initializing AI agents
```

---

# Adoption

For a new project:

1. Read the Core Principles.
2. Read the Development Flow.
3. Read the Development Horizons.
4. Read the Decision Authority.
5. Assign project roles.
6. Copy the required templates.
7. Bootstrap the Lead Orchestrator.
8. Start with the Product Roadmap.

For an existing project:

See:

- `docs/project-adoption.md`

---

# AI Agents

PEOS treats AI agents as members of the engineering organization.

Typical roles include:

- Lead Orchestrator
- Principal Engineer
- Senior Engineer
- Documentation Agent
- Testing Agent
- Domain Specialist

Agents may propose solutions, but they never redefine product vision, architecture or technical strategy without explicit human approval.

---

# Templates

PEOS provides reusable templates for common engineering artifacts, including:

- Product Brief
- Product Roadmap
- MVP Scope
- Epic Specification
- ADR
- Implementation Proposal
- PR Review

Projects are encouraged to extend these templates while preserving the PEOS workflow.

---

# Design Goals

PEOS aims to:

- improve product quality
- reduce architectural drift
- make AI collaboration predictable
- keep documentation aligned with reality
- make implementation reviewable
- separate product decisions from implementation work
- create a repeatable engineering workflow across projects

---

# Scope

PEOS intentionally does not prescribe:

- programming languages
- frameworks
- cloud providers
- AI providers
- deployment platforms
- version control systems

Those choices belong to each project.

PEOS defines the engineering process—not the technology stack.

---

# Status

PEOS is developed using PEOS itself.

The methodology is continuously validated and refined through real-world projects.

Current validation projects include:

- PickOne
- Daily Commit

PEOS evolves only when real projects expose opportunities to improve the process.