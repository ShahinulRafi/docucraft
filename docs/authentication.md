---
title: "Authentication"
date: "2026-10-14"
parent: "introduction"
order: 2
author: "Alex B"
category: "Security"
tags: ["authentication", "api-key", "security"]
---

## API Authentication

Protocol uses API keys to authenticate requests and identify applications.

### API Keys

Every application receives a unique API key. Include this key in the Authorization header of your requests.

### Authorization Header

```http
Authorization: Bearer YOUR_API_KEY
```

### Security Recommendations

- Never expose API keys in frontend code.
- Store credentials in environment variables.
- Rotate compromised API keys immediately.
- Use HTTPS for all API requests.

### Authentication Errors

If your API key is missing or invalid, the server returns a `401 Unauthorized` response.
