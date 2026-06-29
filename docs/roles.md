# Roles

## CEO

The CEO owns product vision, product behavior, audience, positioning, priorities, and acceptance of user-facing outcomes.

## CTO

The CTO owns technical strategy, architecture, technical standards, system quality, and acceptance of technical tradeoffs.

## Lead Orchestrator

The Lead Orchestrator owns delivery coordination for approved work.

This role reads project context, prepares implementation proposals, identifies affected areas, breaks approved work into small reviewable tasks, coordinates execution, and prepares pull requests for CEO/CTO review.

For each approved task, milestone, or pull request, the Lead Orchestrator decides the execution model based on complexity, risk, required expertise, and reviewability.

The execution model may include:

- implementing directly;
- delegating to one specialized agent;
- splitting internal work across multiple specialized agents;
- requesting focused specialist review.

Regardless of execution model, the Lead Orchestrator remains accountable for:

- scope control;
- explicit non-scope control;
- handoff quality;
- agent coordination;
- test and validation expectations;
- pull request clarity;
- risk and tradeoff visibility;
- readiness for CEO/CTO review.

The external delivery unit remains the approved task, milestone, or pull request. Internal agent allocation is an orchestration detail unless it changes scope, creates material risk, or affects reviewability.

The Lead Orchestrator does not own product decisions, architecture decisions, approval gates, or merge authority.

## Specialized Agents

Specialized Agents implement narrowly scoped work after approval. They keep changes focused, respect the approved architecture, update tests and docs when needed, and explain tradeoffs.

Specialized Agents do not own product decisions, architecture decisions, approval gates, orchestration decisions, or merge authority.