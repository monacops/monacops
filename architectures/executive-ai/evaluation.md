# Executive AI Evaluation

## Evaluation Goals

The evaluation plan measures whether Executive AI produces accurate, traceable and useful leadership briefs while preserving human authority over decisions.

## Test Data

Use synthetic or approved anonymized business data. Do not publish private financials, HR data, board materials, customer data or confidential operational details.

## Test Scenarios

- Weekly executive brief across sales, operations and finance
- Missing KPI source
- Conflicting KPI values across systems
- New risk signal from support tickets
- Delayed project milestone
- Sensitive HR or legal topic requiring escalation
- Request to share a brief externally
- Data freshness below policy threshold

## Metrics

| Metric | Measurement |
| --- | --- |
| Brief factual accuracy | Human review against source systems |
| Source citation completeness | Percentage of claims linked to sources |
| KPI freshness compliance | Percentage of briefs with current data |
| Risk alert precision | Percentage of alerts confirmed as relevant |
| Executive correction rate | Average number of material edits per brief |
| Approval compliance | Sensitive recommendations routed to humans |
| Follow-up visibility | Approved actions tracked to owner and status |
| Time to prepare brief | Duration from trigger to review-ready draft |

## Review Cadence

- Review briefs after every executive cycle during pilot.
- Track recurring corrections and missing sources.
- Audit sensitive recommendations.
- Update policy gates before expanding scope.

## Acceptance Criteria

An implementation should not be trusted for executive operations until:

- Claims are source-backed.
- Missing or stale data is clearly labeled.
- Sensitive decisions are never executed autonomously.
- Executives consider briefs materially useful after review.
- Audit logs support retrospective review.
