# ADR-004 Store app data locally in SQLite

### Status

Decision accepted for Phase 2

### Context

FairShare must retain transactions and budgets between app launches and use them for reports. The team selected local SQLite; no account, remote database, or sync is required by the project brief.

### Decision

Use Expo SQLite to store transactions, categories, and budgets locally in the Android app sandbox. Keep the first version fully offline without remote services, login, or cloud sync. Do not collect bank credentials or card numbers; use synthetic demo data. Treat this as a course prototype, not a secure finance product.

### Consequences

- Data stays on one device and is not automatically synced or restored.
- This choice does not add database encryption; do not use real financial data.
- Define a small schema and test Android reads and writes. Revisit encryption and backup if real data becomes a requirement.
