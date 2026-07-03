# RevLeak Billing Audit

RevLeak is a fixed-scope forensic billing exception audit for SaaS and subscription businesses.

It checks sanitized CSV exports from contracts/order forms, invoices, usage, credits, and amendments, then returns:

- a Markdown executive report,
- an exceptions CSV,
- normalized input summaries,
- a row-level evidence ledger for operator review.

The implementation is private. This public page is only a buyer-safe overview and sample-output preview.

## What The Audit Finds

- Active accounts with usage or contracted revenue but no invoice.
- Invoices below contract-derived expected billing.
- Usage overages that may be missing or undercharged.
- Failed or unpaid invoices.
- Duplicate invoice events.
- Usage without active contract coverage.

## Sample Demo Results

Canonical sample:

- 12 exceptions found.
- 5 high severity.
- $2,441 high/medium amount to inspect.

Messy client-export sample:

- 9 exceptions found.
- 4 high severity.
- $2,728 high/medium amount to inspect.

## First-Client Pricing

- $49 small export-set audit.
- $99 standard 24-hour audit.
- $199 expanded audit with operator recommendations.

No production credentials are required. Sanitized customer IDs are enough.

## Request An Audit

Open the `RevLeak audit request` issue form with only non-sensitive context:

- company type,
- billing system,
- whether you have contracts/order forms, invoices, usage, credits, and amendments as CSV,
- preferred contact method.

Do not upload private exports publicly. Review the HTML sample report at https://jagadish-645.github.io/revleak-audit/sample-report.html

