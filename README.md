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

## First-Client Pricing

- $49 small export-set audit.
- $99 standard 24-hour audit.
- $199 expanded audit with operator recommendations.
- INR 999 India emergency cleanup for one CSV/XLSX file or exception check, UPI-friendly after sanitized shape check.

No production credentials are required. Sanitized customer IDs are enough.

## Fast Approval Path

For the shortest path, email `jagadish.goudaa@gmail.com` with:

```text
I approve a $49 first-client RevLeak audit if my sanitized export shape is auditable.

Billing system:
Exports available:
Turnaround: 24 hours after sanitized exports are received
```

Do not attach raw exports, credentials, payment-card data, or private customer data in public channels. Send sanitized headers or fake/anonymized sample rows first.

## India Emergency Cleanup

For India-based founders, finance teams, CAs, and operators:

```text
I approve an INR 999 emergency CSV/XLSX cleanup or exception check if my sanitized file shape is doable.

File type:
Problem:
Turnaround: 24 hours after sanitized file is received
```

Payment details are handled only after the free shape check confirms the task is doable. Do not send PAN, Aadhaar, bank statements, credentials, payroll PII, or private customer data in the first message.

## Request An Audit

Open the `RevLeak audit request` issue form with only non-sensitive context:

https://github.com/jagadish-645/revleak-audit/issues/new?template=audit_request.yml

- company type,
- billing system,
- whether you have contracts/order forms, invoices, usage, credits, and amendments as CSV,
- preferred contact method.

Do not upload private exports publicly. Review the HTML sample report at https://jagadish-645.github.io/revleak-audit/sample-report.html
