# Test Plan — Atelier QA41

## Purpose
Define the scope, approach, environment, and completion criteria for manual testing of the SauceDemo demonstration shopping application.

## Application under test
- URL: https://www.saucedemo.com/
- Type: Demonstration e-commerce web application
- Approach: Black-box manual testing through the browser
- No application source code or production data was accessed or modified.

## Objectives
- Verify key customer journeys and input validation.
- Check inventory display, product sorting, cart operations, and checkout.
- Exercise navigation, logout, and session behaviour.
- Explore edge cases and usability.
- Record actual behaviour and report reproducible defects.

## In scope
1. Login and authentication
2. Inventory and product details
3. Product sorting
4. Shopping cart
5. Checkout and form validation
6. Navigation
7. Logout and session behaviour
8. Cart and checkout edge cases
9. UI and usability
10. Exploratory testing

API testing is a separate Postman practice exercise under `api-testing/` and is not included in the manual execution totals.

## Out of scope
- Source-code review or white-box testing
- Production payment processing or real purchases
- Load, stress, and performance benchmarking
- Security penetration testing
- Cross-browser certification beyond the recorded browser session
- Vendor-side fix verification

## Test environment
- Device: Desktop
- OS: Windows (exact version not recorded)
- Browser: Google Chrome (exact version not recorded)
- Test data: Public demo account and fictitious checkout details
- Execution date recorded: 2026-11-03 (IST)

## Test design and execution
- Use positive, negative, boundary, and exploratory scenarios.
- Execute tests manually through the application UI.
- Compare actual behaviour with expected results in the test cases.
- Record Pass, Fail, Blocked, or Not Run.
- Capture screenshots for noteworthy failures where possible.
- Create a defect report for reproducible deviations.

## Entry criteria
- SauceDemo is reachable.
- A demo account is available.
- Browser is available.
- Test cases are prepared.

## Exit criteria
- Planned manual checks have been attempted.
- Results are recorded in the execution log.
- Identified defects have reproducible reports.
- A summary report communicates coverage, results, and limitations.

## Defect handling
Record a unique ID, preconditions, reproduction steps, expected result, actual result, evidence, and proposed severity/priority. Severity and priority remain proposed until reviewed against formal requirements and product impact.

## Risks and limitations
- SauceDemo is a public demo and may change without notice.
- Demo behaviour may not represent a production e-commerce system.
- Exact browser and OS versions were not captured.
- Most execution results were tester-reported; evidence images are not all stored in the repository.
- Recheck the empty-cart finding on the current demo before drawing conclusions beyond this test session.
