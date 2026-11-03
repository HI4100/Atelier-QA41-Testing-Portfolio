# Functional Test Cases — SauceDemo

Application: https://www.saucedemo.com/

## Login and authentication

| ID | Test | Steps | Expected result | Status |
|---|---|---|---|---|
| SD-LOGIN-001 | Valid login | Enter standard demo username and matching password; click Login. | Inventory page opens. | Pass |
| SD-LOGIN-002 | Both fields empty | Leave username and password empty; click Login. | Login is prevented and required-field validation appears. | Pass |
| SD-LOGIN-003 | Empty username | Leave username empty, enter password; click Login. | Login is prevented with username-required validation. | Pass |
| SD-LOGIN-004 | Empty password | Enter username, leave password empty; click Login. | Login is prevented with password-required validation. | Pass |
| SD-LOGIN-005 | Invalid username | Enter an invalid username and password; click Login. | Login is rejected with an authentication error. | Pass |
| SD-LOGIN-006 | Incorrect password | Enter valid demo username and incorrect password; click Login. | Login is rejected with an authentication error. | Pass |
| SD-LOGIN-007 | Locked account | Enter documented locked-out demo username and password; click Login. | Login is blocked with an explanatory message. | Pass |

### Observed messages
- LOGIN-002: "Epic sadface: Username is required"
- LOGIN-003: "Epic sadface: Username is required"
- LOGIN-004: "Epic sadface: Password is require" (transcribed as reported; check screenshot for exact spelling)
- LOGIN-005 and LOGIN-006: "Epic sadface: Username and password do not match any user in this service"
- LOGIN-007: "Epic sadface: Sorry, this user has been locked out."

## Remaining functional test cases

| ID | Feature | Test steps | Expected result | Status |
|---|---|---|---|---|
| SD-INV-001 | Inventory | Log in and inspect product listing. | Product cards display product information and actions. | Not Run |
| SD-INV-002 | Sorting | Select each available sort option. | Products reorder according to selected option. | Not Run |
| SD-CART-001 | Cart | Add one product to cart. | Cart indicator updates and product appears in cart. | Not Run |
| SD-CART-002 | Cart | Remove an added product. | Cart indicator and contents update. | Not Run |
| SD-CART-003 | Cart | Open cart after adding multiple products. | Cart shows selected products and visible details. | Not Run |
| SD-CHECKOUT-001 | Checkout | Submit checkout form with required fields empty. | Validation prevents progression. | Not Run |
| SD-CHECKOUT-002 | Checkout | Enter fictitious demo information and continue. | User proceeds to order overview. | Not Run |
| SD-CHECKOUT-003 | Checkout | Review overview and finish order. | Confirmation page is displayed. | Not Run |
| SD-NAV-001 | Navigation | Use app controls to return to inventory. | User returns to expected page without unexpected error. | Not Run |
| SD-LOGOUT-001 | Logout | Open menu and select Logout. | Login page is displayed. | Not Run |

Use only demo credentials published by SauceDemo. Never store passwords, tokens, or personal data in this repository. Record actual observations; do not infer success.
