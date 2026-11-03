# API Testing with Postman

This folder contains a prepared REST API practice suite for JSONPlaceholder.

## Important

JSONPlaceholder is a public fake REST API for learning and prototyping. POST, PUT, PATCH, and DELETE responses simulate API behaviour; they do not permanently change the service's stored data. Do not use real credentials or personal data.

The collection is **prepared but has not been formally executed in Postman**. The response bodies for API-001 and API-002 were independently spot-checked; their HTTP status codes, response times and automated Postman assertions were not captured. API-003 through API-007 remain pending. Do not count any of these checks as formal Postman passes until the collection has been run and its results recorded.

## Import into Postman

1. Open Postman.
2. Select **Import**.
3. Import `postman/Atelier-QA41-API-Testing.postman_collection.json`.
4. Import `postman/Atelier-QA41-API-Environment.postman_environment.json`.
5. Select the imported environment named **Atelier QA41 — JSONPlaceholder**.
6. Open the collection and select **Run**.
7. Run the requests in order and inspect the response and test results for each request.

## Included requests

- GET a post by ID — verify HTTP 200 and response fields.
- GET the posts collection — verify HTTP 200 and array response.
- POST a new post — verify HTTP 201 and submitted values in the response.
- PUT an existing post — verify HTTP 200 and updated values in the response.
- PATCH an existing post — verify HTTP 200 and the changed field.
- DELETE an existing post — verify successful deletion response.
- GET an invalid route — verify HTTP 404.

## What to record

For each request, record:
- HTTP method and endpoint
- Expected and actual status code
- Response time (if available)
- Response body/schema checks
- Postman test result (pass/fail)
- Any defect or unexpected response

## Learning outcomes

This exercise practises HTTP methods, status codes, JSON response validation, request bodies, environment variables, and Postman test scripts.
