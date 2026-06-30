# Decision Authority

## Purpose

This document defines who owns each type of decision within PEOS.

Clear ownership prevents duplicated responsibilities, conflicting decisions and unnecessary discussions.

Every significant decision should have a single owner.

---

# Principles

Decision ownership is different from implementation ownership.

Owning a decision does not necessarily mean implementing it.

Likewise, implementing something does not grant authority to redefine previously approved decisions.

When uncertainty arises, decisions should always move upward through the organization.

---

# Decision Matrix

| Decision | Owner |
|-----------|-------|
| Product Vision | CEO |
| Product Roadmap | CEO |
| Product Prioritization | CEO |
| Epic Specification | CEO + CTO |
| Product Acceptance | CEO |
| Technical Strategy | CTO |
| Architecture | CTO |
| ADRs | CTO |
| Technical Acceptance | CTO |
| Implementation Proposal | Lead Orchestrator |
| Epic Decomposition into Work Packages | Lead Orchestrator |
| Work Package Assignment | Lead Orchestrator |
| Work Package Technical Review | Principal Engineer |
| Work Package Approval | Principal Engineer |
| Production Code | Specialized Agents |
| Tests | Specialized Agents |
| Documentation Updates | Specialized Agents |
| Epic Pull Request | Lead Orchestrator |
| Final Merge | CEO + CTO |
| PEOS Evolution | CEO + CTO |

---

# Responsibilities by Role

## CEO

Owns all product decisions.

Examples:

- Product Vision
- Product Roadmap
- Product Priorities
- User Experience
- Product Acceptance

The CEO does not participate in implementation decisions.

---

## CTO

Owns all technical decisions.

Examples:

- Architecture
- Technical Strategy
- ADRs
- Technical Acceptance

The CTO does not review individual implementation Pull Requests.

Instead, the CTO validates that completed Epics remain aligned with the approved technical strategy.

---

## Lead Orchestrator

Owns execution planning.

Examples:

- Implementation Proposal
- Work Package planning
- Agent coordination
- Epic progress tracking
- Epic Pull Request creation

The Lead Orchestrator never changes product or technical decisions.

---

## Principal Engineer

Owns technical quality during implementation.

Examples:

- Review every Work Package Pull Request
- Request implementation changes
- Validate architectural consistency
- Ensure implementation quality
- Approve Work Package Pull Requests

The Principal Engineer ensures that implementation remains faithful to the approved architecture and the intent of the Epic.

---

## Specialized Agents

Own implementation.

Examples:

- Production code
- Tests
- Refactoring
- Documentation updates

Specialized Agents never redefine architecture or product behaviour.

Whenever implementation reveals uncertainty, they escalate the issue through the organization.

---

# Escalation Path

Questions should always move upward.

Implementation should always move downward.

```text
Specialized Agent
        ↓
Lead Orchestrator
        ↓
Principal Engineer
        ↓
CTO
        ↓
CEO
```

Only decisions move upward.

Implementation flows downward.

---

# Decision Rules

- Product decisions belong to the CEO.
- Technical decisions belong to the CTO.
- Execution planning belongs to the Lead Orchestrator.
- Technical implementation quality belongs to the Principal Engineer.
- Implementation belongs to Specialized Agents.
- No role may redefine a decision owned by another role.
- Human approval is always required before implementation begins.