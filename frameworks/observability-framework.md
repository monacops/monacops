# Observability Framework

Observability makes agent behavior understandable, measurable and reviewable.

## What To Observe

- Workflow trigger and request context
- Agent decisions and routing
- Data sources retrieved
- Tool calls and integration outcomes
- Policy checks
- Human approvals and rejections
- Generated outputs and revisions
- Latency and failure states
- Evaluation results over time

## Core Signals

| Signal | Purpose |
| --- | --- |
| Trace ID | Connects each workflow step across systems |
| Agent identity | Shows which agent performed each action |
| Source references | Supports factual review |
| Tool call log | Records integrations used and parameters passed |
| Approval event | Shows who approved or rejected sensitive actions |
| Policy event | Records blocked, escalated or permitted actions |
| Confidence and uncertainty | Helps humans prioritize review |
| Failure reason | Enables incident review and improvement |

## Dashboards

Recommended dashboards:

- Workflow volume and completion rate
- Approval queue latency
- Failure and fallback rate
- Policy gate activations
- Tool and integration errors
- Draft acceptance and edit rate
- Evaluation quality trends
- Data freshness and missing-source warnings

## Review Practices

- Review high-risk workflows frequently during pilots.
- Sample approved, rejected and failed actions.
- Compare automated outputs with human-reviewed ground truth.
- Investigate recurring errors before expanding scope.
- Keep observability data private and access-controlled.
