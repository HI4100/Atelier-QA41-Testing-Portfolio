# API Test Cases — JSONPlaceholder

**Base URL:** https://jsonplaceholder.typicode.com  
**Tool:** Postman  
**Execution status:** Not run — collection prepared for tester execution.

| ID | Method | Endpoint | Scenario | Expected result |
|---|---|---|---|---|
| API-001 | GET | /posts/1 | Retrieve one existing post. | 200; JSON object includes id, userId, title, body. |
| API-002 | GET | /posts | Retrieve posts collection. | 200; JSON array with post objects. |
| API-003 | POST | /posts | Create a practice post with JSON body. | 201; response echoes submitted title/body/userId and includes an id. |
| API-004 | PUT | /posts/1 | Replace an existing practice post. | 200; response contains submitted replacement fields. |
| API-005 | PATCH | /posts/1 | Update the title of a practice post. | 200; response contains updated title. |
| API-006 | DELETE | /posts/1 | Send a delete request for a practice post. | 200; response indicates simulated successful deletion. |
| API-007 | GET | /invalid-endpoint | Request an unknown route. | 404. |

## Execution recording template

| ID | Actual status | Response time | Postman assertions | Result | Notes |
|---|---|---|---|---|---|
| API-001 | Not run | — | Not run | Not run | |
| API-002 | Not run | — | Not run | Not run | |
| API-003 | Not run | — | Not run | Not run | |
| API-004 | Not run | — | Not run | Not run | |
| API-005 | Not run | — | Not run | Not run | |
| API-006 | Not run | — | Not run | Not run | |
| API-007 | Not run | — | Not run | Not run | |

## Notes

- JSONPlaceholder is a fake API for testing and prototyping.
- Write operations are simulated and are not persisted.
- Status expectations are based on the service's documented practice behaviour; verify current responses when executing.
