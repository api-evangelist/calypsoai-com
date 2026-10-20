---
name: calypsoai-com-create-chat
description: Create a new chat and retrieve its details.
api: openapi/calypsoai-com-openapi.json
operations:
- post_chats
- get_chats_chatId
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/calypsoai-com-openapi.json ; every operationId checked against the contract
---

# calypsoai-com-create-chat

Create a new chat and retrieve its details.

## Steps

1. 1. Use `post_chats` with the request body fields required to create a chat.
2. 2. Use `get_chats_chatId` with the `chatId` returned from the creation step to fetch the chat details.

## Rules

- Include an `Authorization: Bearer <token>` header as required by the HTTPBearer auth scheme.
