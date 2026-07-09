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
- Buyer-safe sample exceptions CSV: https://jagadish-645.github.io/revleak-audit/sample-exceptions.csv

## Scoped Diagnostic Request

Use this page as a proof sample, not as a place to send private data.

If the sample matches a real billing, export, or exception-ledger problem, email `jagadish.goudaa@gmail.com` with:

```text
I have a billing/export exception problem that may fit RevLeak.

Billing system:
Exports available as CSV:
What looks wrong:
Decision deadline:
```

No production credentials are required. Do not attach raw exports, credentials, payment-card data, bank data, payroll PII, or private customer data in public channels. Send sanitized headers or fake/anonymized sample rows first. A paid scope is quoted only after the export shape is confirmed auditable.

## Request An Audit

Open the `RevLeak audit request` issue form with only non-sensitive context:

https://github.com/jagadish-645/revleak-audit/issues/new?template=audit_request.yml

- company type,
- billing system,
- whether you have contracts/order forms, invoices, usage, credits, and amendments as CSV,
- preferred contact method.

Do not upload private exports publicly. Review the HTML sample report at https://jagadish-645.github.io/revleak-audit/sample-report.html
