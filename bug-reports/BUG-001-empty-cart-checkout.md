# BUG-001 — Checkout permits an empty cart

- **Application:** SauceDemo
- **Area:** Cart / Checkout
- **Test case:** SD-EDGE-002
- **Status:** Open
- **Severity:** Major (proposed)
- **Priority:** Medium (proposed)
- **Reproduction environment:** Windows desktop, Google Chrome (exact OS/browser versions not recorded)

## Summary

The application permits a user to proceed through checkout with no products in the cart and displays an empty order overview with $0.00 totals.

## Preconditions

1. User is logged in with a standard SauceDemo demo account.
2. Shopping cart contains zero products.

## Steps to reproduce

1. Open https://www.saucedemo.com/.
2. Log in with a standard demo account.
3. Ensure the cart is empty (use Reset App State if needed).
4. Open the cart.
5. Select **Checkout**.
6. Enter fictitious first name, last name, and postal code.
7. Select **Continue**.

## Expected result

The application should prevent progression and display a clear validation message instructing the user to add at least one product before checkout.

## Actual result

The application opens the **Checkout: Overview** page with no product rows and displays:
- Item total: $0
- Tax: $0.00
- Total: $0.00

## Impact

A user can reach an order overview without selecting any products. This creates an invalid empty-order state and weakens the checkout flow's business validation.

## Evidence

Screenshots of the empty checkout information page and the resulting empty order overview were supplied by the tester during the project conversation. They have not been committed as repository image attachments.

## Reproducibility

Observed by the tester during the manual edge-case execution. Re-test on the current demo application before treating the behaviour as a permanent production defect, since the target is a public demo environment.

## Classification note

Severity **Major** and priority **Medium** are proposed classifications for this portfolio exercise. They are not official vendor classifications.

## Linked GitHub issue

https://github.com/HI4100/Atelier-QA41-Testing-Portfolio/issues/1
