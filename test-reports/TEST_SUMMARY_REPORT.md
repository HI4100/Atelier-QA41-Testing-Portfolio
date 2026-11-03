# Test Summary Report — Atelier QA41

## 1. Project information

| Field | Details |
|---|---|
| Project | Atelier QA41 — Software Testing Portfolio |
| Application under test | https://www.saucedemo.com/ |
| Tester | Humza Warsi |
| Test type | Manual functional, UI, session, edge-case and exploratory testing |
| Execution date recorded | 2026-11-03 (IST; exact execution times not recorded) |
| Environment | Windows desktop, Google Chrome (exact versions not recorded) |

## 2. Objective

Evaluate key user journeys in the SauceDemo demonstration shopping application, record observed results, and document any deviations from expected behaviour.

## 3. Scope

Testing covered login/authentication, inventory/product details, sorting, cart operations, checkout validation, navigation, logout/session behaviour, cart/checkout edge cases, UI/usability, and exploratory checks.

## 4. Execution summary

| Metric | Count |
|---|---:|
| Total checks executed | 50 |
| Passed | 49 |
| Failed | 1 |
| Blocked | 0 |
| Not run | 0 |

Pass rate: **98%** (49 of 50 checks). This is a count-based pass rate for the manual checks recorded in this project.

## 5. Results by category

| Category | Executed | Passed | Failed |
|---|---:|---:|---:|
| Login and authentication | 7 | 7 | 0 |
| Inventory and product listing | 6 | 6 | 0 |
| Product sorting | 5 | 5 | 0 |
| Shopping cart | 7 | 7 | 0 |
| Checkout | 7 | 7 | 0 |
| Navigation | 5 | 5 | 0 |
| Logout and session | 4 | 4 | 0 |
| Cart/checkout edge cases | 4 | 3 | 1 |
| UI and usability | 3 | 3 | 0 |
| Exploratory | 2 | 2 | 0 |
| **Total** | **50** | **49** | **1** |

## 6. Defect summary

### BUG-001 — Checkout permits an empty cart

- **Test case:** SD-EDGE-002
- **Observed behaviour:** Checkout information can be submitted with an empty cart; the overview displays no product rows and $0.00 totals.
- **Expected behaviour:** Checkout should be blocked and the user should be prompted to add a product.
- **Severity:** Major (proposed)
- **Priority:** Medium (proposed)
- **Tracking:** https://github.com/HI4100/Atelier-QA41-Testing-Portfolio/issues/1

## 7. Test conclusion

The manual test run exercised 50 checks. Forty-nine matched the expected outcomes recorded for the test run. One check exposed the empty-cart checkout behaviour and has been documented as BUG-001.

The project demonstrates a structured manual testing workflow: test-case execution, result recording, defect identification, and defect reporting. The findings are limited to the public demo application and the recorded test environment.

## 8. Limitations and follow-up

- Browser and operating-system version numbers were not captured.
- Most manual outcomes were supplied as tester-reported observations; screenshots were shared for selected checks but are not all stored in the repository.
- The empty-cart behaviour should be rechecked against a formal requirement and on a fresh session before any production-impact claim.
- API tests are supplied as a Postman practice collection but have not yet been executed; they are excluded from the 50 manual checks and 98% pass rate.
- Retesting after a vendor-side fix is outside the scope of this execution.

## 9. Deliverables

- Functional test cases: `test-cases/functional-test-cases.md`
- Execution log: `test-execution/TEST_EXECUTION_LOG.md`
- Defect report: `bug-reports/BUG-001-empty-cart-checkout.md`
- Postman collection and environment: `api-testing/postman/`
