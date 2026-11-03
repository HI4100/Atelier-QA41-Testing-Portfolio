# Functional Test Cases — SauceDemo

Application: https://www.saucedemo.com/

**Execution status: Not executed yet. Change statuses only after performing each test.**

| ID | Feature | Steps | Expected result | Type | Status |
|---|---|---|---|---|---|
| SD-LOGIN-001 | Login | Enter a valid demo username and password; select Login. | User reaches inventory page. | Positive | Not Run |
| SD-LOGIN-002 | Login | Submit with username and password empty. | Required-field validation appears; login is not completed. | Negative | Not Run |
| SD-LOGIN-003 | Login | Enter valid username and invalid password. | Login is rejected with a clear error. | Negative | Not Run |
| SD-LOGIN-004 | Login | Enter unknown username and a password. | Login is rejected; inventory is not shown. | Negative | Not Run |
| SD-LOGIN-005 | Login | Use a locked demo account if listed by the site. | Login is blocked with an explanatory message. | Negative | Not Run |
| SD-INV-001 | Inventory | Log in and inspect product listing. | Product cards display product information and actions. | Positive | Not Run |
| SD-INV-002 | Sorting | Select each available sort option. | Products reorder according to selected option. | Functional | Not Run |
| SD-CART-001 | Cart | Add one product to cart. | Cart indicator updates and product appears in cart. | Positive | Not Run |
| SD-CART-002 | Cart | Remove an added product. | Cart indicator and contents update. | Positive | Not Run |
| SD-CART-003 | Cart | Open cart after adding multiple products. | Cart shows selected products and visible details. | Positive | Not Run |
| SD-CHECKOUT-001 | Checkout | Submit checkout form with required fields empty. | Validation prevents progression. | Negative | Not Run |
| SD-CHECKOUT-002 | Checkout | Enter fictitious demo information and continue. | User proceeds to order overview. | Positive | Not Run |
| SD-CHECKOUT-003 | Checkout | Review overview and finish order. | Confirmation page is displayed. | Positive | Not Run |
| SD-NAV-001 | Navigation | Use app controls to return to inventory. | User returns to expected page without unexpected error. | Functional | Not Run |
| SD-LOGOUT-001 | Logout | Open menu and select Logout. | Login page is displayed. | Positive | Not Run |

## Test data
Use only demo credentials explicitly published by SauceDemo. Do not store passwords, tokens, or personal data. Use fictitious checkout values.

## Execution rules
Record observations; do not infer success. For failures, retry once in a fresh session unless deterministic. Record browser/OS and date. Preserve IDs once assigned.
