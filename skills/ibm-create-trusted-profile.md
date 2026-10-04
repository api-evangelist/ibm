---
name: ibm-create-trusted-profile
description: Create a new trusted profile and retrieve its details.
api: openapi/ibm-trusted-profiles-api-openapi.yml
operations:
- createProfile
- getProfile
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/ibm-trusted-profiles-api-openapi.yml ; every operationId checked against the contract
---

# ibm-create-trusted-profile

Create a new trusted profile and retrieve its details.

## Steps

1. 1. Use `createProfile` with the request body containing the profile attributes (e.g., `name`, `description`, `account_id`).
2. 2. Use `getProfile` with the path parameter `profile-id` returned from the create step to fetch the created profile.

## Rules

- Authentication: Include an `Authorization: Bearer <token>` header (bearerAuth).
