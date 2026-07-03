# RevLeak Sample Audit Report

Billing period: 2026-06

This is a demo report generated from synthetic SaaS billing exports. It shows the shape of the paid deliverable without exposing implementation details.

## Executive Summary

- Exceptions found: 9
- High severity: 4
- Medium severity: 5
- Estimated high/medium amount to inspect: $2,728.00

This is an exception ledger for operator review. It is not accounting advice, revenue-recognition advice, or a guarantee that every exception is collectible.

## Exception Preview

| Rule | Severity | Customer | Issue | Est. Amount | Evidence Summary |
| --- | --- | --- | --- | ---: | --- |
| RLK-002 | High | Corelytics (C103) | Invoice is below contract-derived expected amount | $340.00 | Latest invoice billed $1,700.00; expected $2,040.00 after usage, credits, and discounts. |
| RLK-002 | High | Atlas Docs (C101) | Invoice is below contract-derived expected amount | $120.00 | Latest invoice billed $600.00; expected $720.00 after usage, credits, and discounts. |
| RLK-001 | High | DeltaDesk (C104) | Active account has usage or contracted revenue but no invoice | $120.00 | Expected billing for 2026-06 is $120.00; no invoice found. |
| RLK-004 | Medium | Corelytics (C103) | Invoice is not marked paid | $1,700.00 | Invoice BILL-8803 status is `past_due`. |
| RLK-007 | Medium | C199 (C199) | Usage exists without an active contract | $0.00 | Usage=2500 in 2026-06, but no active contract was found. |

## Recommended Operator Workflow

1. Review high-severity rows against signed order forms and billing-system line items.
2. Check whether amendments were applied before the invoice date.
3. Validate whether credits are valid, expired, or accidentally duplicated.
4. Re-run before the next billing cycle with fresh exports.

