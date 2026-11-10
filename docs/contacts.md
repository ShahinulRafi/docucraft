---
title: "Contacts"
date: "2026-10-16"
parent: "api-reference"
order: 1
author: "Alex B"
category: "API Reference"
tags: ["contacts", "users", "endpoints"]
---

## Contacts API

The Contacts API allows you to create, retrieve, update, and delete contacts.

### Get All Contacts

`GET /v1/contacts`

Returns a list of contacts associated with your application.

### Get a Single Contact

`GET /v1/contacts/{contact_id}`

Retrieves information about a specific contact.

### Create a Contact

`POST /v1/contacts`

Example request:

```json
{
  "name": "John Doe",
  "email": "john@example.com"
}
```

### Delete a Contact

`DELETE /v1/contacts/{contact_id}`

Permanently removes a contact from your application.
