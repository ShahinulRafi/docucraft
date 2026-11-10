---
title: "Messages"
date: "2026-10-18"
parent: "api-reference"
order: 3
author: "Alex B"
category: "API Reference"
tags: ["messages", "chat", "endpoints"]
---

## Messages API

The Messages API allows you to send and retrieve messages within conversations.

### Send a Message

`POST /v1/messages`

Example request:

```json
{
  "conversation_id": "conv_101",
  "content": "Hello, everyone!"
}
```

### Retrieve Messages

`GET /v1/conversations/{conversation_id}/messages`

Returns messages belonging to a specific conversation.

### Message Structure

Each message contains an ID, sender, content, timestamp, and conversation ID.
