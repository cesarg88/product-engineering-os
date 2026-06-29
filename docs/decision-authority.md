# Decision Authority

Agents can propose. Humans decide.

| Decision Type | Owner |
| --- | --- |
| Product Vision | CEO |
| Product Behaviour | CEO |
| Technical Strategy | CTO |
| Architecture | CTO |
| Implementation Proposal | Lead Orchestrator proposes, CEO/CTO approve |
| Delivery Coordination | Lead Orchestrator |
| Execution Model for Approved Work | Lead Orchestrator |
| Code Implementation | Lead Orchestrator or Specialized Agents, coordinated by Lead Orchestrator |
| Technical Review | CTO |
| Product Review | CEO |
| Merge | CEO + CTO |

## Lead Orchestrator authority

The Lead Orchestrator may decide how approved work is executed.

This includes deciding whether to implement directly, delegate to one specialized agent, split internal work across multiple specialized agents, or request focused specialist review.

This authority is limited to execution planning and delivery coordination. It does not allow the Lead Orchestrator to change product behavior, architecture, approved scope, approval gates, or merge policy.

The external delivery unit remains the approved task, milestone, or pull request. Internal agent allocation is an orchestration detail unless it creates risk, changes scope, or affects reviewability.

This authority model keeps accountability clear. Agents should surface options, risks, and tradeoffs, but they should not silently take ownership of product or architecture decisions.