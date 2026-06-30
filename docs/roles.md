# Roles

## Purpose

This document defines the responsibilities and decision authority of every role in PEOS.

Each role owns a specific part of the development process.

Responsibilities should never overlap unless explicitly stated.

---

# CEO

## Purpose

Owns the product.

The CEO is responsible for ensuring the product solves the right problem and delivers value to users.

## Responsibilities

- Product Vision
- Product Roadmap
- Epic Specification
- Product Prioritization
- Product Acceptance

The CEO does not participate in implementation details.

---

# CTO

## Purpose

Owns the technical strategy.

The CTO ensures the product remains technically coherent and maintainable over time.

## Responsibilities

- Technical Strategy
- Architecture
- Technical Decisions
- ADRs
- Technical Acceptance

The CTO does not review every implementation Pull Request.

Instead, the CTO validates that each completed Epic remains aligned with the approved technical strategy.

---

# Lead Orchestrator

## Purpose

Owns execution planning.

The Lead Orchestrator translates approved product and technical decisions into an executable implementation plan.

## Responsibilities

- Read approved documentation
- Produce the Implementation Proposal
- Decompose Epics into Work Packages
- Coordinate Specialized Agents
- Track implementation progress
- Open the final Epic Pull Request

The Lead Orchestrator does not redefine product or architecture.

---

# Principal Engineer

## Purpose

Owns technical quality during implementation.

The Principal Engineer ensures every Work Package remains aligned with the approved architecture and the intent of the Epic.

## Responsibilities

- Review the Implementation Proposal
- Review every Work Package Pull Request
- Request changes when necessary
- Ensure architectural consistency
- Ensure implementation quality
- Validate test coverage
- Approve Work Package Pull Requests

The Principal Engineer does not redefine product goals or technical strategy.

Those responsibilities belong to the CEO and CTO.

---

# Specialized Agents

## Purpose

Implement approved Work Packages.

## Responsibilities

- Production code
- Tests
- Documentation updates
- Refactoring
- Bug fixes

Specialized Agents never redefine architecture or product behaviour.

When implementation reveals uncertainty, they escalate it to the Lead Orchestrator.

---

# Responsibility Summary

| Role | Main Responsibility |
|------|---------------------|
| CEO | Product |
| CTO | Technical Strategy |
| Lead Orchestrator | Execution Planning |
| Principal Engineer | Technical Quality During Delivery |
| Specialized Agents | Implementation |

---

# Escalation Path

Questions should always move upward through the organization.

Specialized Agent

↓

Lead Orchestrator

↓

Principal Engineer

↓

CTO

↓

CEO

Only decisions move upward.

Implementation should always move downward.