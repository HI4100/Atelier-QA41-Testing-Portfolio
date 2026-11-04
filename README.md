# ATELIER 41 | QA Testing Portfolio

A beginner QA testing portfolio built around hands-on functional, UI, session, exploratory, and API testing practice using the public SauceDemo demo application.

**Tester:** Humza Warsi  
**Primary application under test:** https://www.saucedemo.com/  
**API practice service:** https://jsonplaceholder.typicode.com/

## Project objectives

- Design and execute structured manual test cases.
- Validate login, inventory, sorting, cart, checkout, navigation, logout, UI, and session behaviour.
- Record actual outcomes and distinguish passed tests from defects.
- Create reproducible bug reports with steps, expected and actual results, and evidence.
- Practise REST API testing with Postman.

## Current manual test results

| Metric | Result |
|---|---:|
| Manual checks executed | 50 |
| Passed | 49 |
| Failed | 1 |
| Blocked | 0 |
| Not run | 0 |

The single failed check is **SD-EDGE-002**: SauceDemo allows checkout to proceed with an empty cart and displays an empty order overview with $0.00 totals. This is documented as BUG-001. Severity and priority are proposed QA assessments and should be reviewed against formal product requirements.

Results are based on the tester's reported observations during manual execution. Screenshots were shared in the working conversation; they have not all been committed as image files in this repository.

## Test coverage

- Login and authentication
- Inventory and product details
- Product sorting
- Shopping cart
- Checkout and field validation
- Navigation
- Logout and session behaviour
- Cart and checkout edge cases
- UI and usability
- Exploratory testing

## Repository structure

```text
.
├── README.md
├── test-cases/
│   └── functional-test-cases.md
├── test-execution/
│   └── TEST_EXECUTION_LOG.md
├── bug-reports/
│   └── BUG-001-empty-cart-checkout.md
├── test-reports/
│   └── TEST_SUMMARY_REPORT.md
└── api-testing/
    ├── README.md
    ├── postman/
    │   ├── Atelier-QA41-API-Testing.postman_collection.json
    │   └── Atelier-QA41-API-Environment.postman_environment.json
    └── API_TEST_CASES.md
```

## API testing

The Postman collection uses JSONPlaceholder, a public fake REST API intended for practice. Its write endpoints simulate create/update/delete responses; changes are not permanently stored. The collection is prepared for import and execution, but its requests have **not** been represented as executed or passed in this report. Follow the instructions in [API testing](api-testing/README.md).

## How to use

0. Read the [test plan](TEST_PLAN.md).
1. Read the [functional test cases](test-cases/functional-test-cases.md).
2. Review the [test execution log](test-execution/TEST_EXECUTION_LOG.md).
3. Read the [BUG-001 defect report](bug-reports/BUG-001-empty-cart-checkout.md).
4. Review the [final manual test summary](test-reports/TEST_SUMMARY_REPORT.md).
5. Import the Postman collection and environment from `api-testing/postman/` and execute the API practice tests.

## Scope and limitations

This is a learning and portfolio project, not a formal certification or an independent audit. The manual test results are based on the tester's observations. No source code or internal implementation of SauceDemo was modified. The API collection is a prepared practice suite and requires execution in Postman before results can be claimed.

## Author

**Humza Warsi**  
GitHub: https://github.com/HI4100


---

## ✨ ATELIER 41 Signature

> **Build it clearly. Test it carefully. Document it honestly. Improve it continuously.**

This project is part of my **ATELIER 41** portfolio — a connected collection of practical projects built and documented by **Humza Warsi**.

🔗 GitHub: [@HI4100](https://github.com/HI4100) • ✨ **ATELIER 41**


---

## ✨ ATELIER 41 | Portfolio Signature

**Build it clearly. Test it carefully. Document it honestly. Improve it continuously.**

Created and maintained as part of the **ATELIER 41** project series by **Humza Warsi**.

- Portfolio: [github.com/HI4100](https://github.com/HI4100)
- Project source: [ATELIER 41 — QA Testing Portfolio](https://github.com/HI4100/Atelier-QA41-Testing-Portfolio)

**Attribution & reuse:** This repository is published as a learning and portfolio project. Please retain this attribution and the project history when referencing or adapting the work. Do not present this repository or its original work as your own. Check the repository license before reusing code or other materials.
