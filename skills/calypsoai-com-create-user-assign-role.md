---
name: calypsoai-com-create-user-assign-role
description: Create a new user and assign a role to the user.
api: openapi/calypsoai-com-openapi.json
operations:
- post_users
- post_users_userId_roles_roleId
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/calypsoai-com-openapi.json ; every operationId checked against the contract
---

# calypsoai-com-create-user-assign-role

Create a new user and assign a role to the user.

## Steps

1. 1. Call `post_users` with the request body fields required to create the user (e.g., email, password, name).
2. 2. Call `post_users_userId_roles_roleId` with the path parameters `userId` (returned from step 1) and `roleId` (the role to assign).

## Rules

- Include an `Authorization: Bearer <token>` header for all requests (HTTPBearer auth).
- The `post_users` operation is not idempotent; avoid duplicate calls.
- If the user creation fails, handle HTTP 4xx/5xx error responses as defined by the API.
