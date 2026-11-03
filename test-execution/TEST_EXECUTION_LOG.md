# Test Execution Log — Atelier QA41

## Environment
- Application: https://www.saucedemo.com/
- Tester: Humza Warsi
- Date recorded: 2026-11-03 (IST; exact execution times not recorded)
- Device: Desktop
- Operating system: Windows (exact version not recorded)
- Browser: Google Chrome (exact version not recorded)
- Test approach: Manual black-box browser testing
- Evidence: Selected screenshots were shared in the working conversation. Not all screenshots have been committed to this repository.

## Execution results by category

| Category | Checks | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login and authentication | 7 | 7 | 0 | 0 | 0 |
| Inventory and product listing | 6 | 6 | 0 | 0 | 0 |
| Product sorting | 5 | 5 | 0 | 0 | 0 |
| Shopping cart | 7 | 7 | 0 | 0 | 0 |
| Checkout | 7 | 7 | 0 | 0 | 0 |
| Navigation | 5 | 5 | 0 | 0 | 0 |
| Logout and session | 4 | 4 | 0 | 0 | 0 |
| Cart/checkout edge cases | 4 | 3 | 1 | 0 | 0 |
| UI and usability | 3 | 3 | 0 | 0 | 0 |
| Exploratory | 2 | 2 | 0 | 0 | 0 |
| **Overall** | **50** | **49** | **1** | **0** | **0** |

**Manual pass rate: 98% (49/50).**

## Detailed edge-case results

| Test Case ID | Status | Actual result | Evidence |
|---|---|---|---|
| SD-EDGE-001 | Pass | Opened cart with no products; tester reported empty-cart view behaved as expected. | Tester-reported |
| SD-EDGE-002 | **Fail — BUG-001** | Checkout proceeded with an empty cart. Overview displayed no product rows and showed Item total $0, Tax $0.00, Total $0.00. | Screenshots supplied in conversation |
| SD-EDGE-003 | Pass | Added a product, removed it, and added it again; tester reported cart state updated correctly. | Tester-reported |
| SD-EDGE-004 | Pass | Added multiple products and checked item count/order summary; tester reported expected behaviour. | Tester-reported |

## Defect reference

**BUG-001 — Checkout permits an empty cart and displays a $0.00 order.**

Expected: prevent checkout and prompt the user to add at least one product.

Actual: allow progression to an empty order overview with $0.00 totals.

- GitHub issue: https://github.com/HI4100/Atelier-QA41-Testing-Portfolio/issues/1
- Full report: [bug-reports/BUG-001-empty-cart-checkout.md](../bug-reports/BUG-001-empty-cart-checkout.md)
- Severity: Major (proposed)
- Priority: Medium (proposed)
- Status: Open

## Notes and limitations
- Manual outcomes are based on the tester's reported observations; selected screenshots were supplied for evidence.
- Exact OS and browser version numbers were not captured.
- The application is a public demo and may change. Recheck BUG-001 before making claims about later versions.
- API collection is prepared for Postman but has not been executed. API tests are excluded from the 50 manual checks and 98% pass rate.
