# Development Horizons

PEOS uses five horizons as the canonical workflow definition. They keep product intent, technical direction, delivery, review, and merge authority separate.

Project Adoption may happen once before the horizons begin. After adoption, projects never return to Project Adoption; all subsequent work starts at H1.

## Workflow Overview

```text
Project Created
  |
  v
Project Adoption (only once if required)
  |
  v
H1 Product Vision
  |
  v
H2 Technical Strategy
  |
  v
H3 Delivery
  |
  v
H4 Technical Review
  |
  v
H5 Merge
  |
  v
Repeat
```

## H1 — Product Vision

Purpose

Define what product outcome should be pursued and why.

Owner

CEO.

Expected Output

Approved product direction, behavior, or work item.

Exit Condition

Product decision approved.

## H2 — Technical Strategy

Purpose

Define how the approved product work will be implemented.

Owner

CTO owns technical strategy. Lead Orchestrator proposes implementation. CEO and CTO approve.

Expected Output

Approved Implementation Proposal.

Exit Condition

Implementation Proposal approved. No code is written before this approval.

## H3 — Delivery

Purpose

Implement the approved proposal in small, focused changes.

Owner

Specialized Agents implement. Lead Orchestrator coordinates.

Expected Output

Pull Request opened with implementation, tests, and relevant documentation updates.

Exit Condition

Pull Request ready for review.

## H4 — Technical Review

Purpose

Review architecture, maintainability, tests, risk, and technical fit.

Owner

CTO.

Expected Output

Technical review decision.

Exit Condition

Technical review approved or changes requested and resolved.

## H5 — Merge

Purpose

Confirm product and technical readiness before the work enters the project.

Owner

CEO and CTO.

Expected Output

Merged work or explicit decision not to merge.

Exit Condition

Merge completed. The next work item starts again at H1.

## State Transitions

| Current State | Event | Next State |
| --- | --- | --- |
| Project Created | Adoption required | Project Adoption |
| Project Created | No adoption required | H1 |
| Project Adoption | Bootstrap Proposal approved | H1 |
| H1 Product Vision | Product decision approved | H2 Technical Strategy |
| H2 Technical Strategy | Implementation Proposal approved | H3 Delivery |
| H3 Delivery | Pull Request opened | H4 Technical Review |
| H4 Technical Review | Review approved | H5 Merge |
| H4 Technical Review | Changes requested | H3 Delivery |
| H5 Merge | Merge completed | H1 Product Vision |
