# Test Plan — SauceDemo

## 1. Objective
Validate key user-facing workflows of the SauceDemo demonstration shopping application and maintain traceable test documentation.

## 2. Scope

### In scope
- Login and logout behaviour
- Product inventory page and product details
- Product sorting
- Add/remove items in cart
- Cart contents and navigation
- Checkout form validation and order flow
- Basic usability observations and cross-page navigation

### Out of scope
- Load, stress, and denial-of-service testing
- Penetration testing or exploitation
- Testing against real customer accounts or real payments
- Claims about internal implementation that cannot be observed

## 3. Test approach
Use manual black-box testing. Derive test cases from observable functionality and execute them in a normal browser session. Include positive, negative, boundary, and regression cases where appropriate.

## 4. Test environment
Record the actual browser, browser version, operating system, device/viewport, date and application URL in the execution log before reporting results. Do not guess environment details.

## 5. Entry criteria
- Public demo site is reachable.
- Test scope and test cases are documented.
- A supported browser is available.

## 6. Exit criteria
- Planned test cases have an execution status.
- Failed or blocked tests include clear notes.
- Any reported defect is reproducible and has steps, expected result, actual result, and evidence.
- Summary counts match the execution log.

## 7. Severity guide
- **Critical:** Core service unusable or major data/security impact.
- **High:** Major workflow blocked with no reasonable workaround.
- **Medium:** Important feature incorrect, workaround exists.
- **Low:** Minor UI, content, or cosmetic issue.

Severity is impact; priority is urgency and should be assessed separately.

## 8. Risks and constraints
The demo application may change, be unavailable, or behave differently by browser/session. Record the date and environment to make observations reproducible. Use only demo-provided accounts and data.

## 9. Deliverables
Test scenarios, detailed test cases, execution log, reproducible bug reports, evidence references, and (later) API test documentation.
