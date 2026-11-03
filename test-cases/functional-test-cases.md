# Functional Test Cases — SauceDemo

**Application:** https://www.saucedemo.com/  
**Execution status:** Not executed yet. Update statuses only after performing each test.

| Test Case ID | Feature | Test steps | Expected result | Type | Status |
|---|---|---|---|---|---|
| SD-LOGIN-001 | Login | Enter a valid demo username and password; select Login. | User reaches the inventory page. | Positive | Not Run |
| SD-LOGIN-002 | Login | Submit with both username and password empty. | Required-field validation is shown; login is not completed. | Negative | Not Run |
| SD-LOGIN-003 | Login | Enter a valid username and an invalid password. | Login is rejected with a clear error message. | Negative | Not Run |
| SD-LOGIN-004 | Login | Enter an unknown username and a password. | Login is rejected; inventory page is not shown. | Negative | Not Run |
| SD-LOGIN-005 | Login | Enter a locked demo account, if provided by the site's login information. | Login is blocked with an explanatory message. | Negative | Not Run |
| SD-INV-001 | Inventory | Log in and inspect the product listing. | Product cards display product information and available actions. | Positive | Not Run |
| SD-INV-002 | Sorting | Select each available sort option. | Products are reordered according to the selected option. | Functional | Not Run |
| SD-CART-001 | Cart | Add one product to the cart. | Cart indicator updates and product appears in cart. | Positive | Not Run |
| SD-CART-002 | Cart | Remove an added product from the inventory page. | Cart indicator and cart contents update accordingly. | Positive | Not Run |
| SD-CART-003 | Cart | Open cart after adding multiple different products. | Cart shows the selected products and correct visible details. | Positive | Not Run |
| SD-CHECKOUT-001 | Checkout | Proceed to checkout and submit the form with required fields empty. | Required-field validation prevents progression. | Negative | Not Run |
| SD-CHECKOUT-002 | Checkout | Enter valid demo checkout information and continue. | User proceeds to the order overview. | Positive | Not Run |
| SD-CHECKOUT-003 | Checkout | Review the order overview and finish the order. | Confirmation page is displayed. | Positive | Not Run |
| SD-NAV-001 | Navigation | Use the app's navigation controls to return to inventory. | User returns to the expected page without an unexpected error. | Functional | Not Run |
| SD-LOGOUT-001 | Logout | Log in, open the menu and select Logout. | Login page is displayed and protected content is no longer accessible in that session. | Positive | Not Run |

## Test data notes
Use only demo credentials explicitly published by SauceDemo. Do not store passwords, tokens, personal data, or secret values in this repository. For checkout, use clearly fictitious demo values accepted by the application.

## Execution rules
- Capture actual observations; do not infer success from the expected result.
- For any failure, retry once in a fresh session before reporting, unless the issue is clearly deterministic.
- Record browser/OS and date in the execution log.
- Add new rows for additional test cases; preserve test case IDs once used.
