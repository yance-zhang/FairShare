# ADR-002 Use simple tabs and a page stack with Expo Router

### Status

Decision accepted for Phase 2

### Context

FairShare has four main areas: dashboard, transactions, budgets, and reports. Entry and edit forms are secondary tasks.

### Decision

Use Expo Router with bottom tabs for Dashboard, Transactions, Budgets, and Reports. Add a simple stack route for transaction details and add/edit forms. Keep Settings reachable from the Dashboard. Use Android back to return to the prior screen; avoid nested navigation complexity.

### Consequences

- Follow Expo Router route-file conventions.
- Keep a predictable return path from transaction forms.
- Test the four tabs, add/edit flow, and Android back behavior.