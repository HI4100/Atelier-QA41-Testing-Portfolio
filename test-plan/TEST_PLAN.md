# Test Plan — SauceDemo

## Objective
Validate key user-facing workflows of the SauceDemo demonstration shopping application and maintain traceable test documentation.

## Scope
In scope: login/logout, inventory and details, sorting, cart operations, checkout validation and order flow.

Out of scope: load/stress/denial-of-service testing, penetration testing or exploitation, real customer accounts/payments, and claims about unobservable internal implementation.

## Approach
Manual black-box testing using positive, negative, boundary, and regression cases derived from observable functionality.

## Environment
Record actual browser/version, operating system, device/viewport, date/time, and application URL in the execution log. Do not guess environment details.

## Entry criteria
- Public demo site is reachable.
- Test scope and test cases are documented.

## Exit criteria
- Every planned test has an execution status.
- Failed or blocked tests include notes.
- Defects are reproducible and include steps, expected/actual results, and evidence.
- Summary counts match the execution log.

## Severity guide
- Critical: core service unusable or major data/security impact.
- High: major workflow blocked with no reasonable workaround.
- Medium: important feature incorrect; workaround exists.
- Low: minor UI, content, or cosmetic issue.

Severity measures impact; priority measures urgency.

## Risks and constraints
The demo application may change or be unavailable. Record date and environment for reproducibility. Use only demo-provided accounts and data.

## Deliverables
Test scenarios, detailed cases, execution log, reproducible bug reports, evidence references, and later API test documentation.
