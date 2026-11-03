# Test Execution Log

## Environment
- Application URL: https://www.saucedemo.com/
- Date: 2026-11-03 (IST; exact execution time not recorded)
- Operating system: Windows desktop (exact version not verified)
- Browser: Google Chrome (version not verified)
- Device: Desktop
- Tester: Humza Warsi

## Login test execution results
| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-LOGIN-001 | 2026-11-03 | Pass | Valid demo login succeeded; inventory page and product cards appeared. | Screenshot shared in conversation |
| SD-LOGIN-002 | 2026-11-03 | Pass | Empty username and password returned: "Epic sadface: Username is required". | Tester-reported result |
| SD-LOGIN-003 | 2026-11-03 | Pass | Empty username with password entered returned: "Epic sadface: Username is required". | Tester-reported result |
| SD-LOGIN-004 | 2026-11-03 | Pass | Username entered with empty password returned: "Epic sadface: Password is require" (transcribed as reported). | Tester-reported result |
| SD-LOGIN-005 | 2026-11-03 | Pass | Invalid username returned: "Epic sadface: Username and password do not match any user in this service". | Tester-reported result |
| SD-LOGIN-006 | 2026-11-03 | Pass | Valid username with incorrect password returned: "Epic sadface: Username and password do not match any user in this service". | Tester-reported result |
| SD-LOGIN-007 | 2026-11-03 | Pass | Locked demo account returned: "Epic sadface: Sorry, this user has been locked out." | Tester-reported result |

## Inventory test execution results
| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-INV-001 | 2026-11-03 | Pass | Tester reported inventory loaded correctly. | Tester-reported result |
| SD-INV-002 | 2026-11-03 | Pass | Tester reported product names and descriptions were correct. | Tester-reported result |
| SD-INV-003 | 2026-11-03 | Pass | Tester reported product prices were displayed correctly. | Tester-reported result |
| SD-INV-004 | 2026-11-03 | Pass | Tester reported product images loaded correctly. | Tester-reported result |
| SD-INV-005 | 2026-11-03 | Pass | Product detail view displayed Sauce Labs Backpack name, description, image, price ($29.99), and Add to cart control. | Screenshot shared in conversation |
| SD-INV-006 | 2026-11-03 | Pass | Tester reported return to inventory worked correctly. | Tester-reported result |

## Summary
| Category | Total | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login | 7 | 7 | 0 | 0 | 0 |
| Inventory | 6 | 6 | 0 | 0 | 0 |
| **Overall executed** | **13** | **13** | **0** | **0** | **0** |

A tester-reported result is distinguished from a screenshot-backed observation in the evidence column.
