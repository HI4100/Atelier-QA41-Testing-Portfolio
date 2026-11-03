# API Test Cases — JSONPlaceholder

**Base URL:** https://jsonplaceholder.typicode.com  
**Tool intended for formal execution:** Postman  
**Current status:** Collection prepared. Two GET response bodies were independently inspected; the full collection has not been run in Postman.

## Test cases and results

| ID | Method | Endpoint | Scenario | Expected result | Current result |
|---|---|---|---|---|---|
| API-001 | GET | /posts/1 | Retrieve one existing post. | HTTP 200; JSON object includes id, userId, title and body. | **Response body verified** — expected post fields were present. HTTP status and response time were not captured in a Postman run. |
| API-002 | GET | /posts | Retrieve the posts collection. | HTTP 200; JSON array containing post objects. | **Response body verified** — response was an array of post objects. HTTP status and response time were not captured in a Postman run. |
| API-003 | POST | /posts | Create a practice post with a JSON request body. | HTTP 201; response echoes submitted title/body/userId and includes an id. | **Pending execution** — expected behaviour only; not reported as a pass. |
| API-004 | PUT | /posts/1 | Replace an existing practice post. | HTTP 200; response contains submitted replacement fields. | **Pending execution** — expected behaviour only; not reported as a pass. |
| API-005 | PATCH | /posts/1 | Update the title of a practice post. | HTTP 200; response contains updated title. | **Pending execution** — expected behaviour only; not reported as a pass. |
| API-006 | DELETE | /posts/1 | Send a delete request for a practice post. | HTTP 200; response indicates simulated successful deletion. | **Pending execution** — expected behaviour only; not reported as a pass. |
| API-007 | GET | /invalid-endpoint | Request an unknown route. | HTTP 404. | **Pending execution** — expected behaviour only; not reported as a pass. |

## Execution record

| ID | Response inspection | Actual HTTP status | Response time | Postman assertions | Formal result |
|---|---|---|---|---|---|
| API-001 | JSON object and required fields observed | Not captured | Not captured | Not run | Not run |
| API-002 | JSON array and post objects observed | Not captured | Not captured | Not run | Not run |
| API-003 | Not performed | — | — | Not run | Pending |
| API-004 | Not performed | — | — | Not run | Pending |
| API-005 | Not performed | — | — | Not run | Pending |
| API-006 | Not performed | — | — | Not run | Pending |
| API-007 | Not performed | — | — | Not run | Pending |

## Interpretation

- The two GET response bodies were inspected as a basic endpoint spot-check. This was not a formal Postman collection run, and no HTTP status code, response time, or automated assertion result was captured.
- The other five scenarios are documented with expected outcomes only. They must remain pending until executed.
- No API pass rate is calculated because a complete, formal execution has not been performed.
- These API checks are separate from the 50 manual SauceDemo checks reported in the main test summary.

## Notes

- JSONPlaceholder is a fake REST API for testing and prototyping.
- POST, PUT, PATCH and DELETE operations are simulated and are not persistently stored.
- Status-code expectations are test expectations, not claimed observations, for pending scenarios.
