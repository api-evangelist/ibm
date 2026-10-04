---
name: ibm-create-and-list-policies
description: Create a new access policy and then retrieve the list of policies.
api: openapi/ibm-policies-api-openapi.yml
operations:
- createPolicy
- listPolicies
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/ibm-policies-api-openapi.yml ; every operationId checked against the contract
---

# ibm-create-and-list-policies

Create a new access policy and then retrieve the list of policies.

## Steps

1. 1. `createPolicy` – request body fields not specified in the documentation.
2. 2. `listPolicies` – query parameters not specified in the documentation.

## Rules

- Auth: Include a Bearer token in the Authorization header (bearerAuth).
