# Functional Test Cases — SauceDemo

Application: https://www.saucedemo.com/  
Execution status: Manual checks completed on 2026-11-03. See [execution log](../test-execution/TEST_EXECUTION_LOG.md).

## Login and authentication

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-LOGIN-001 | Log in with standard demo credentials. | Inventory page opens. | Pass |
| SD-LOGIN-002 | Submit with both fields empty. | Login prevented; username-required validation appears. | Pass |
| SD-LOGIN-003 | Submit with username empty and password entered. | Username-required validation appears. | Pass |
| SD-LOGIN-004 | Submit with username entered and password empty. | Password-required validation appears. | Pass |
| SD-LOGIN-005 | Submit invalid username and password. | Authentication rejected. | Pass |
| SD-LOGIN-006 | Submit valid username and incorrect password. | Authentication rejected. | Pass |
| SD-LOGIN-007 | Submit credentials for documented locked demo account. | Login blocked with explanatory message. | Pass |

## Inventory and product listing

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-INV-001 | Inspect inventory after login. | Inventory and product cards load. | Pass |
| SD-INV-002 | Inspect product names and descriptions. | Product text is visible and correct. | Pass |
| SD-INV-003 | Inspect product prices. | Prices are visible. | Pass |
| SD-INV-004 | Inspect product images. | Images load. | Pass |
| SD-INV-005 | Open a product detail page. | Product name, description, image, price and action are displayed. | Pass |
| SD-INV-006 | Select Back to products. | Inventory page is displayed again. | Pass |

## Product sorting

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-SORT-001 | Select Name (A to Z). | Products sort alphabetically ascending. | Pass |
| SD-SORT-002 | Select Name (Z to A). | Products sort alphabetically descending. | Pass |
| SD-SORT-003 | Select Price (low to high). | Prices sort ascending. | Pass |
| SD-SORT-004 | Select Price (high to low). | Prices sort descending. | Pass |
| SD-SORT-005 | Change sort options repeatedly. | Product order updates correctly each time. | Pass |

## Shopping cart

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-CART-001 | Add one product. | Cart indicator updates and product appears. | Pass |
| SD-CART-002 | Add a second product. | Cart count updates to two. | Pass |
| SD-CART-003 | Open cart after adding multiple products. | Selected products and details appear. | Pass |
| SD-CART-004 | Remove one of two cart products. | Remaining product stays in cart. | Pass |
| SD-CART-005 | Remove all cart products. | Cart becomes empty. | Pass |
| SD-CART-006 | Select Continue Shopping. | Inventory page opens. | Pass |
| SD-CART-007 | Add several products and inspect names/prices. | Cart displays selected product details correctly. | Pass |

## Checkout

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-CHECKOUT-001 | Click Checkout from cart. | Checkout information page opens. | Pass |
| SD-CHECKOUT-002 | Submit all checkout fields empty. | Required-field validation prevents progression. | Pass |
| SD-CHECKOUT-003 | Enter first name only and continue. | Last-name validation prevents progression. | Pass |
| SD-CHECKOUT-004 | Enter first and last name but omit postal code. | Postal-code validation prevents progression. | Pass |
| SD-CHECKOUT-005 | Enter fictitious valid information and continue. | Order overview opens. | Pass |
| SD-CHECKOUT-006 | Review product details and displayed totals. | Values are consistent with cart and displayed calculations. | Pass |
| SD-CHECKOUT-007 | Select Finish. | Order confirmation page appears. | Pass |

## Navigation

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-NAV-001 | Open hamburger menu. | Navigation menu appears. | Pass |
| SD-NAV-002 | Select All Items. | Inventory page opens. | Pass |
| SD-NAV-003 | Select About. | Expected external page opens. | Pass |
| SD-NAV-004 | Select Continue Shopping from cart. | Inventory page opens. | Pass |
| SD-NAV-005 | Use browser Back and Forward during navigation. | Navigation behaves as expected. | Pass |

## Logout and session

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-LOGOUT-001 | Select Logout from hamburger menu. | Login page appears. | Pass |
| SD-LOGOUT-002 | Use browser Back after logout. | Active logged-in session is not restored. | Pass |
| SD-LOGOUT-003 | Refresh login page. | Login page remains available. | Pass |
| SD-LOGOUT-004 | Log in again with standard demo credentials. | New session opens successfully. | Pass |

## Cart and checkout edge cases

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-EDGE-001 | Open cart without adding products. | Empty cart is displayed. | Pass |
| SD-EDGE-002 | Attempt checkout with an empty cart. | Checkout is blocked and user is prompted to add at least one product. | **Fail — BUG-001** |
| SD-EDGE-003 | Add a product, remove it, then add it again. | Cart state updates correctly. | Pass |
| SD-EDGE-004 | Add multiple products and inspect count and order summary. | Item count and summary match selected products. | Pass |

## UI and usability

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-UI-001 | Inspect application for broken or missing images. | Images load correctly. | Pass |
| SD-UI-002 | Check buttons and links for visibility and usability. | Controls are visible and usable. | Pass |
| SD-UI-003 | Resize browser window and inspect layout. | Layout remains usable at tested window sizes. | Pass |

## Exploratory testing

| ID | Test | Expected result | Status |
|---|---|---|---|
| SD-EXP-001 | Refresh inventory page after login. | Session and inventory remain available. | Pass |
| SD-EXP-002 | Use Reset App State from the menu. | Cart contents and application state reset. | Pass |

## Test result summary

- Total manual checks: 50
- Passed: 49
- Failed: 1 (SD-EDGE-002 / BUG-001)
- Blocked: 0
- Not run: 0

Use only demo credentials published by SauceDemo. Never store passwords, tokens, or personal data in this repository.
