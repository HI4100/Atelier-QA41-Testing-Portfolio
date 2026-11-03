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


## Product sorting test execution results

| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-SORT-001 | 2026-11-03 | Pass | Name (A to Z) selected; tester reported sorting worked correctly. | Tester-reported result |
| SD-SORT-002 | 2026-11-03 | Pass | Name (Z to A) selected; tester reported sorting worked correctly. | Tester-reported result |
| SD-SORT-003 | 2026-11-03 | Pass | Price (low to high) selected; tester reported sorting worked correctly. | Tester-reported result |
| SD-SORT-004 | 2026-11-03 | Pass | Price (high to low) selected; screenshot shows descending price order beginning with $49.99 then $29.99, followed by $15.99 items. | Screenshot shared in conversation |
| SD-SORT-005 | 2026-11-03 | Pass | Tester changed sorting options several times and reported that the order updated correctly. | Tester-reported result |

## Updated summary
| Category | Total | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login | 7 | 7 | 0 | 0 | 0 |
| Inventory | 6 | 6 | 0 | 0 | 0 |
| Product sorting | 5 | 5 | 0 | 0 | 0 |
| **Overall executed** | **18** | **18** | **0** | **0** | **0** |


## Shopping cart test execution results

| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-CART-001 | 2026-11-03 | Pass | Added one product; tester reported expected cart behaviour. | Tester-reported result |
| SD-CART-002 | 2026-11-03 | Pass | Added a second product; tester reported cart count updated correctly. | Tester-reported result |
| SD-CART-003 | 2026-11-03 | Pass | Opened cart; tester reported both products appeared. | Tester-reported result |
| SD-CART-004 | 2026-11-03 | Pass | Removed one product; tester reported remaining product stayed in cart. | Tester-reported result |
| SD-CART-005 | 2026-11-03 | Pass | Removed all products; tester reported cart became empty. | Tester-reported result |
| SD-CART-006 | 2026-11-03 | Pass | Returned to inventory using Continue Shopping; tester reported navigation worked. | Tester-reported result |
| SD-CART-007 | 2026-11-03 | Pass | Added several products and checked names/prices; tester reported details were correct. | Tester-reported result |

## Updated summary
| Category | Total | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login | 7 | 7 | 0 | 0 | 0 |
| Inventory | 6 | 6 | 0 | 0 | 0 |
| Product sorting | 5 | 5 | 0 | 0 | 0 |
| Shopping cart | 7 | 7 | 0 | 0 | 0 |
| **Overall executed** | **25** | **25** | **0** | **0** | **0** |


## Checkout test execution results

| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-CHECKOUT-001 | 2026-11-03 | Pass | Checkout information page opened from the cart. | Tester-reported result |
| SD-CHECKOUT-002 | 2026-11-03 | Pass | Submitting all fields empty displayed "Error: First Name is required". | Screenshot shared in conversation |
| SD-CHECKOUT-003 | 2026-11-03 | Pass | Entering only first name displayed "Error: Last Name is required". | Tester-reported result |
| SD-CHECKOUT-004 | 2026-11-03 | Pass | Entering first and last name without postal code displayed "Error: Postal Code is required". | Tester-reported result |
| SD-CHECKOUT-005 | 2026-11-03 | Pass | Fictitious valid checkout information allowed progression to the order overview. | Tester-reported result |
| SD-CHECKOUT-006 | 2026-11-03 | Pass | Tester reported that product details and displayed totals were correct on the overview. | Tester-reported result |
| SD-CHECKOUT-007 | 2026-11-03 | Pass | Finish completed the demo checkout; confirmation page displayed "Thank you for your order!" | Screenshot shared in conversation |

## Updated summary
| Category | Total | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login | 7 | 7 | 0 | 0 | 0 |
| Inventory | 6 | 6 | 0 | 0 | 0 |
| Product sorting | 5 | 5 | 0 | 0 | 0 |
| Shopping cart | 7 | 7 | 0 | 0 | 0 |
| Checkout | 7 | 7 | 0 | 0 | 0 |
| **Overall executed** | **32** | **32** | **0** | **0** | **0** |


## Navigation test execution results

| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-NAV-001 | 2026-11-03 | Pass | Hamburger menu opened successfully. | Tester-reported result |
| SD-NAV-002 | 2026-11-03 | Pass | All Items selected; inventory page opened successfully. | Tester-reported result |
| SD-NAV-003 | 2026-11-03 | Pass | About selected; expected external page opened successfully. | Tester-reported result |
| SD-NAV-004 | 2026-11-03 | Pass | Continue Shopping returned to inventory successfully. | Tester-reported result |
| SD-NAV-005 | 2026-11-03 | Pass | Browser Back and Forward navigation behaved as expected. | Tester-reported result |

## Updated summary
| Category | Total | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login | 7 | 7 | 0 | 0 | 0 |
| Inventory | 6 | 6 | 0 | 0 | 0 |
| Product sorting | 5 | 5 | 0 | 0 | 0 |
| Shopping cart | 7 | 7 | 0 | 0 | 0 |
| Checkout | 7 | 7 | 0 | 0 | 0 |
| Navigation | 5 | 5 | 0 | 0 | 0 |
| **Overall executed** | **37** | **37** | **0** | **0** | **0** |


## Logout and session test execution results

| Test Case ID | Date | Status | Actual result | Evidence |
|---|---|---|---|---|
| SD-LOGOUT-001 | 2026-11-03 | Pass | Logout selected from the menu; login page appeared. | Tester-reported result |
| SD-LOGOUT-002 | 2026-11-03 | Pass | After logout, browser Back did not restore an active logged-in session. | Tester-reported result |
| SD-LOGOUT-003 | 2026-11-03 | Pass | Refreshing the login page kept the login page available. | Tester-reported result |
| SD-LOGOUT-004 | 2026-11-03 | Pass | Standard demo credentials successfully opened a new session. | Tester-reported result |

## Updated summary

| Category | Total | Passed | Failed | Blocked | Not run |
|---|---:|---:|---:|---:|---:|
| Login | 7 | 7 | 0 | 0 | 0 |
| Inventory | 6 | 6 | 0 | 0 | 0 |
| Product sorting | 5 | 5 | 0 | 0 | 0 |
| Shopping cart | 7 | 7 | 0 | 0 | 0 |
| Checkout | 7 | 7 | 0 | 0 | 0 |
| Navigation | 5 | 5 | 0 | 0 | 0 |
| Logout/session | 4 | 4 | 0 | 0 | 0 |
| **Overall executed** | **41** | **41** | **0** | **0** | **0** |
