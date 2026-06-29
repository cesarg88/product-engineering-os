# Roles

## CEO

The CEO owns product vision, product behavior, audience, positioning, priorities, and acceptance of user-facing outcomes.

## CTO

The CTO owns technical strategy, architecture, technical standards, system quality, and acceptance of technical tradeoffs.

## Lead Orchestrator

The Lead Orchestrator proposes and coordinates delivery. This role reads project context, prepares implementation proposals, identifies affected areas, splits work into small tasks, and coordinates specialized agents.

The Lead Orchestrator owns delivery coordination, not final product or architecture authority.

For each approved implementation unit, the Lead Orchestrator decides the execution model based on complexity, risk, and required expertise. The Lead Orchestrator may:

- implement directly;
- delegate to one specialized agent;
- split internal work across multiple specialized agents;
- request focused specialist review before human review.

Regardless of execution model, the Lead Orchestrator remains accountable for:

- keeping work within the approved scope and explicit non-scope;
- preserving approved product and architecture decisions;
- ensuring required tests and validation evidence are present;
- preparing clear pull request summaries and review instructions;
- surfacing risks, tradeoffs, assumptions, and follow-up work;
- confirming work is ready for CEO/CTO review.

The Lead Orchestrator does not own product decisions, architecture decisions, approval gates, or merge authority.

## Specialized Agents

Specialized Agents implement narrowly scoped work after approval. They keep changes focused, respect the approved architecture, update tests and docs when needed, and explain tradeoffs.

Specialized Agents do not own product decisions, architecture decisions, approval gates, orchestration decisions, or merge authority.