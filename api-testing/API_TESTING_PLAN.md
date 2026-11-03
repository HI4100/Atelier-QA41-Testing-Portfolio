# API Testing Plan

## Status
Planned. No API endpoint has been selected or tested yet.

## Objective
Practice validating HTTP API behaviour: status codes, headers, payload structure, field types, and negative inputs.

## Selection criteria
Choose a public API that explicitly permits demonstration/testing. Review documentation and usage limits. Do not scan arbitrary hosts, bypass authentication, or send high-volume traffic.

## Planned checks
- Correct method and endpoint
- Expected status code
- Response content type
- Required response fields and data types
- Positive and negative inputs
- Missing/invalid parameter handling
- Basic response-time observation (not a load test)

## Evidence to add after execution
- API documentation URL
- Tool and version (e.g. Postman)
- Request method and sanitized URL
- Sanitized request headers/body
- Status code and response body (remove tokens/personal data)
- Actual result and conclusion

Report tests as passed/failed only after sending the request and inspecting the response. Never publish API keys or secrets.
