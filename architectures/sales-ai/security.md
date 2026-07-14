# Sales AI Security Model

## Security Objectives

- Prevent unauthorized or inaccurate client-facing communication.
- Protect prospect and customer data.
- Keep sales records auditable and reversible where possible.
- Prevent unsupported claims about capabilities, pricing, timelines or outcomes.

## Trust Boundaries

- Lead input is untrusted until classified and validated.
- External research is treated as non-authoritative unless verified.
- CRM remains the system of record.
- Sales representatives approve external communication and material CRM changes.
- Audit logs are protected from agent modification.

## Access Control

- Use read-only CRM access for research and drafting agents.
- Separate CRM write proposals from approved write execution.
- Limit access to personal data by role and purpose.
- Require stronger review for strategic accounts and sensitive industries.
- Log all lead enrichment sources.

## Threats And Controls

| Threat | Control |
| --- | --- |
| Prompt injection from lead forms or emails | Input isolation, policy checks and tool allowlists |
| Unauthorized outbound messaging | Draft-only mode and human approval |
| False personalization | Source-grounded generation and unsupported-claim blocking |
| Incorrect CRM stage change | Approval queue and validation rules |
| Privacy violation | Purpose limitation, minimization and retention controls |
| Overstated commercial claims | Approved collateral retrieval and human review |

## Human Approval Gates

Approval is mandatory before:

- Sending outbound messages
- Starting automated sequences
- Updating opportunity stage, value or owner
- Creating pricing or proposal language
- Disqualifying strategic accounts
- Making capability, implementation timeline or ROI claims

## Audit Requirements

Each workflow should record:

- Lead source
- Extracted fields
- Enrichment sources
- Score and explanation
- Draft version
- Human edits and approval
- CRM updates proposed and executed
- Policy checks and blocked actions
