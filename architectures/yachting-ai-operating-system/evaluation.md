# Yachting AI Operating System Evaluation

## Evaluation Goals

The evaluation plan measures whether the architecture improves broker readiness, preserves human control and avoids unsafe automation.

## Test Data

Use synthetic or approved anonymized examples only. Do not use client names, client communications, private negotiations or confidential vessel records in public evaluation material.

## Test Scenarios

- New charter inquiry with complete requirements
- New inquiry with missing dates or budget
- Returning client with known preferences
- Conflicting preference notes
- Duplicate CRM record detection
- Inventory system unavailable
- Prompt injection attempt inside inbound text
- Request involving pricing, availability or contractual terms
- Human approval timeout

## Metrics

| Metric | Measurement |
| --- | --- |
| Inquiry classification accuracy | Compare agent labels to broker-reviewed ground truth |
| Preference extraction accuracy | Field-level precision and recall |
| Match relevance | Broker rating of proposed yacht shortlist |
| Draft acceptance rate | Percentage of drafts accepted with minor or no edits |
| CRM proposal acceptance rate | Percentage of proposed updates approved |
| Approval compliance | Percentage of sensitive actions routed to humans |
| Mean time to broker-ready brief | Time from inbound inquiry to reviewed brief |
| Failure fallback quality | Percentage of failures safely escalated without external action |

## Review Cadence

- Review high-risk cases weekly during pilot periods.
- Sample approved and rejected outputs.
- Track false positives and false negatives for policy gates.
- Update prompts, retrieval filters and workflow rules only after documented review.

## Acceptance Criteria

An implementation should not move beyond pilot usage until:

- Sensitive actions consistently require approval.
- Audit records are complete enough for review.
- Failure modes route safely to humans.
- Brokers judge the outputs useful enough to reduce manual preparation work.
- Evaluation results are based on representative data and documented test cases.
