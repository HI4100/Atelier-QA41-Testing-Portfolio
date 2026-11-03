# Test Execution Log

Fill one row per execution. Results below are based on the tester's reported observations.

## Environment
- Application URL: https://www.saucedemo.com/
- Date/time: 2026-11-03 (IST; exact execution time not recorded for this batch)
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
| SD-LOGIN-004 | 2026-11-03 | Pass | Username entered with empty password returned: "Epic sadface: Password is require" (message transcribed exactly as reported; verify spelling if capturing screenshot). | Tester-reported result |
| SD-LOGIN-005 | 2026-11-03 | Pass | Invalid username returned: "Epic sadface: Username and password do not match any user in this service". | Tester-reported result |
| SD-LOGIN-006 | 2026-11-03 | Pass | Valid username with incorrect password returned: "Epic sadface: Username and password do not match any user in this service". | Tester-reported result |
| SD-LOGIN-007 | 2026-11-03 | Pass | Locked demo account returned: "Epic sadface: Sorry, this user has been locked out." | Tester-reported result |

## Summary — Login category
- Total: 7
- Passed: 7
- Failed: 0
- Blocked: 0
- Not run: 0

Note: "Pass" means the observed behaviour matched the expected outcome for the test. Evidence was reported verbally for LOGIN-002 through LOGIN-007; screenshots were not supplied for those individual tests.
