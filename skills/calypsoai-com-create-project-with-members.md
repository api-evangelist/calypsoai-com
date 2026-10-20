---
name: calypsoai-com-create-project-with-members
description: Create a new project and add users to it.
api: openapi/calypsoai-com-openapi.json
operations:
- post_projects
- post_projects_project_members
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/calypsoai-com-openapi.json ; every operationId checked against the contract
---

# calypsoai-com-create-project-with-members

Create a new project and add users to it.

## Steps

1. 1. Use `post_projects` with body fields: `name`, `description` (if required by the contract).
2. 2. Use `post_projects_project_members` with path parameter `project` (the ID or name returned from step 1) and body fields: `userId`, `role`.

## Rules

- Include an `Authorization: Bearer <token>` header (HTTPBearer auth).
- All POST requests are non‑idempotent; retry only if safe.
