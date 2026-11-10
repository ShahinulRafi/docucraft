---
title: "Rate Limits"
date: "2026-10-24"
parent: "resources"
order: 1
author: "Alex B"
category: "Resources"
tags: ["rate-limits", "performance"]
---

## API Rate Limits

Protocol limits the number of requests an application can make within a specific time window.

### Default Limits

For this example API:

- 100 requests per minute.
- 5,000 requests per hour.

### Rate Limit Headers

Responses may include:

- `X-RateLimit-Limit`
- `X-RateLimit-Remaining`
- `X-RateLimit-Reset`

### Handling Rate Limits

When you receive a `429 Too Many Requests` response, wait before retrying. Use exponential backoff to avoid repeated failures.
