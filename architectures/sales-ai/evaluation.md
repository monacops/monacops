# Sales AI Evaluation

## Evaluation Goals

The evaluation plan measures whether Sales AI improves sales workflow readiness while preserving accuracy, privacy and human control.

## Test Data

Use synthetic or approved anonymized lead records only. Do not publish prospect lists, customer names, private emails, CRM exports or confidential commercial data.

## Test Scenarios

- Complete inbound lead from website form
- Inbound lead with missing company or budget details
- Duplicate lead from an existing account
- Strategic account requiring manager review
- Request involving pricing
- Unsupported performance claim requested by a prospect
- CRM unavailable
- Prompt injection attempt inside inbound message
- Sales representative rejects a draft

## Metrics

| Metric | Measurement |
| --- | --- |
| Lead classification accuracy | Human-reviewed label agreement |
| Field extraction quality | Precision and recall for structured lead fields |
| Duplicate detection accuracy | Confirmed duplicate and non-duplicate outcomes |
| Draft acceptance rate | Accepted drafts with minor or no edits |
| CRM update acceptance rate | Approved proposed updates |
| Response readiness time | Time from lead receipt to approved draft |
| Score calibration | Alignment between agent score and sales manager review |
| Policy compliance | Sensitive actions routed to approval |

## Review Cadence

- Review rejected drafts weekly during pilot.
- Audit all policy gate bypass attempts.
- Compare score recommendations with sales outcomes only after enough real reviewed data exists.
- Update approved collateral and qualification rules when stale.

## Acceptance Criteria

An implementation should not move beyond pilot usage until:

- Outbound communication is consistently approval-gated.
- CRM updates are traceable.
- Drafts avoid unsupported claims.
- Score explanations are useful to sales representatives.
- Failure modes route safely to human review.
