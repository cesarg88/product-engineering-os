# Product Engineering Operating System (PEOS)

> **Build better products by making better decisions before writing code.**

PEOS is an opinionated operating system for AI-assisted product development.

It provides a repeatable workflow for building software products where humans remain responsible for decisions while AI agents accelerate execution.

PEOS is technology-agnostic.

It is not tied to Swift, React, Node.js, OpenAI, Claude, or any specific implementation.

Instead, it defines **how teams think, decide and collaborate** when building products with AI.

---

# Philosophy

PEOS is based on a simple principle:

> Humans own decisions. AI owns execution.

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

These principles define how work flows across the system and who has decision authority.

Start here:

- `docs/core-principles.md`

---

# Development Process

PEOS organizes development into clearly defined horizons.

Each horizon has explicit owners and deliverables.

Typical flow:

```text
Product Vision
        ↓
Technical Strategy
        ↓
Implementation Proposal
        ↓
Delivery
        ↓
Review
        ↓
Merge
```

See:

- `docs/development-horizons.md`
- `docs/decision-authority.md`
- `docs/epic-lifecycle.md`

---

# Repository Structure

```
docs/
    Core principles
    Process
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
2. Read the Development Horizons.
3. Read the Decision Authority.
4. Copy the required templates.
5. Bootstrap your Lead Orchestrator.

For an existing project:

See:

- `docs/project-adoption.md`

---

# AI Agents

PEOS treats AI agents as members of the engineering organization.

Typical roles include:

- Lead Orchestrator
- Senior Engineer
- PR Reviewer
- Documentation Agent
- Testing Agent
- Domain Specialist

Agents may propose solutions, but they never redefine product vision or architecture without explicit approval.

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

---

# Scope

PEOS is intentionally lightweight.

It does not prescribe:

- programming languages
- frameworks
- cloud providers
- AI providers
- deployment platforms

Those choices belong to each project.

PEOS defines the engineering process—not the technology stack.

---

# Status

PEOS is actively evolving through real-world projects.

It is currently being validated while building:

- PickOne
- Daily Commit

Future improvements are expected as the methodology matures through practical use.