---
title: "Conversations"
date: "2026-10-17"
parent: "api-reference"
order: 2
author: "Alex B"
category: "API Reference"
tags: ["conversations", "chat", "endpoints"]
---

## Conversations API

The Conversations API allows you to manage private and group conversations.

### Get Conversations

`GET /v1/conversations`

Returns all conversations accessible to your application.

### Create Conversation

`POST /v1/conversations`

Example request:

```json
{
  "type": "group",
  "participants": ["user_101", "user_102"]
}
```

### Get Conversation Details

`GET /v1/conversations/{conversation_id}`

Returns the details and participants of a conversation.
