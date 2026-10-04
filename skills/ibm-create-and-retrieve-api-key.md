---
name: ibm-create-and-retrieve-api-key
description: Create a new API key and then retrieve its details.
api: openapi/ibm-api-keys-api-openapi.yml
operations:
- createApiKey
- getApiKey
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/ibm-api-keys-api-openapi.yml ; every operationId checked against the contract
---

# ibm-create-and-retrieve-api-key

Create a new API key and then retrieve its details.

## Steps

1. 1. Use `createApiKey` with the request body fields required to define the new API key (e.g., `name`, `description`, `iam_id`).
2. 2. Use `getApiKey` with the path parameter `id` returned from the create step to fetch the newly created API key.

## Rules

- Auth: Include a Bearer token in the `Authorization` header as defined by the `bearerAuth` scheme.
- Pagination: Not applicable for these operations.
- Errors: Follow the HTTP status codes returned by the API (e.g., 4xx for client errors, 5xx for server errors).
