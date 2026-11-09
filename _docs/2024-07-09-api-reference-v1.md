---
title: "API Reference (v1)"
date: 2024-07-09
author: "Ravi Patel"
category: "reference"
status: published
canonical_url: "https://legacy.northwind-docs.example/docs/api-reference-v1"
legacy_id: "NW-1058"
---

# API Reference (v1)

The v1 HTTP API is frozen for backwards compatibility. New capabilities are only
added to the v2 surface.

## Authentication

All requests carry a bearer token issued by the workspace administrator. Tokens
rotate every 90 days and are scoped to a single workspace.

## Rate limits

Bulk endpoints allow 50 requests per second per token. Exceeding the budget
returns `429` with a `Retry-After` header.

## Pagination

Collection endpoints accept `page` and `page_size`. The maximum page size is 100
items; larger values are clamped rather than rejected.

*This page is mirrored from the legacy docs portal at https://legacy.northwind-docs.example/docs/api-reference-v1.*
