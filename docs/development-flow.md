# Development Flow

## Purpose

This document defines the complete lifecycle of an Epic within PEOS.

Every project follows the same flow, regardless of technology stack or AI provider.

---

# Overview

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

Each stage has different owners, deliverables and approval criteria.

---

# Stage 1 — Idea

A new opportunity, problem or improvement is identified.

Owner

- CEO
- CTO

Output

Decision to investigate further.

---

# Stage 2 — Product Roadmap

If accepted, the idea becomes part of the Product Roadmap.

No implementation is discussed.

Question

> Should this become part of the product?

Owner

- CEO
- CTO

Output

Updated Product Roadmap.

---

# Stage 3 — Epic Specification

The Epic is fully defined.

Topics typically include:

- problem
- goals
- user experience
- constraints
- success criteria
- open questions

Question

> What are we building?

Owner

- CEO
- CTO

Output

Epic Specification.

---

# Stage 4 — Technical Strategy

The technical solution is designed.

Typical activities include:

- architecture
- interfaces
- ADRs
- dependencies
- trade-offs
- technical risks

Question

> How should this be built?

Owner

- CTO

Output

Technical Strategy.

---

# Stage 5 — Implementation Proposal

The Lead Orchestrator analyses all approved documentation and produces an execution plan.

No production code is written.

Typical deliverables:

- Work Packages
- implementation order
- affected layers
- testing strategy
- rollout plan
- identified risks

Question

> How should the work be executed?

Owner

- Lead Orchestrator

Output

Implementation Proposal.

---

# Stage 6 — Approval

The Implementation Proposal is reviewed.

Possible outcomes:

- Approved
- Request Changes
- Rejected

Implementation cannot begin until approval has been granted.

Owners

- CEO
- CTO
- Principal Engineer

Output

Approved Implementation Proposal.

---

# Stage 7 — Delivery

The Lead Orchestrator coordinates implementation.

The Epic is decomposed into one or more Work Packages.

Each Work Package is implemented independently.

Typical flow:

```text
Work Package

↓

Implementation Branch

↓

Work Package Pull Request

↓

Principal Engineer Review

↓

Merge into Epic Branch
```

This process is repeated until every Work Package defined in the Implementation Proposal has been completed.

The Lead Orchestrator continuously tracks progress across the Epic.

Once all Work Packages have been completed, the Lead Orchestrator opens a single Epic Pull Request.

The Epic Pull Request contains:

- implementation summary
- completed Work Packages
- testing summary
- documentation updates
- known limitations
- links to all Work Package Pull Requests

Output

Epic Pull Request.

---

# Stage 8 — Epic Acceptance

The Epic is evaluated as a whole.

This is **not** a code review.

Individual Pull Requests have already been reviewed during implementation.

Instead, the Epic is evaluated across four dimensions.

## Product Acceptance

Owner

CEO

Questions

- Does the Epic solve the intended problem?
- Does the user experience match the original vision?
- Are the product goals achieved?

---

## Technical Acceptance

Owner

CTO

Questions

- Is the implementation aligned with the approved architecture?
- Has unnecessary technical debt been introduced?
- Should any new architectural decisions become ADRs?

---

## Documentation Acceptance

Owners

CEO + CTO

Questions

- Is the documentation complete?
- Does it reflect the implemented solution?
- Is the Product Roadmap up to date?

---

## Process Retrospective

Owners

CEO + CTO

Questions

- Did the process work well?
- Did PEOS expose any weaknesses?
- Should PEOS evolve based on this Epic?

Only real project experience may drive changes to PEOS.

Output

Epic Accepted.

---

# Stage 9 — Merge

Once accepted, the Epic Pull Request is merged.

The capability officially becomes part of the product.

Owners

- CEO
- CTO

Output

Merged Epic.

---

# Stage 10 — Documentation Update

Documentation is considered part of the deliverable.

Typical updates include:

- Product Roadmap
- Epic status
- ADRs
- Architecture
- Technical documentation

An Epic is not considered complete until documentation has been synchronized.

---

# Flow Principles

- Product decisions precede implementation.
- Architecture precedes production code.
- AI proposes; humans decide.
- Implementation follows approved documentation.
- Every Work Package is reviewed by the Principal Engineer.
- Every Epic is accepted by the CEO and CTO.
- Documentation is part of the deliverable.
- PEOS evolves only when real projects expose weaknesses.

---

# Related Documents

- Core Principles
- Development Horizons
- Decision Authority
- Roles
- Epic Lifecycle