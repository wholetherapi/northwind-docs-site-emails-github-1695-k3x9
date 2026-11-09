---
title: "Security Hardening Checklist"
date: 2025-02-14
author: "Tomas Novak"
category: "security"
status: published
canonical_url: "https://docs.northwind-labs.example/docs/security-hardening"
migrated: "2026-11-09"
legacy_id: "NW-1090"
---

# Security Hardening Checklist

Run through this checklist before exposing any new service to production traffic.

## Identity

- Require single sign-on for every human-facing surface.
- Issue short-lived credentials for machine identities.
- Rotate service tokens at least every quarter.

## Network

- Default-deny ingress; open ports explicitly with a documented owner.
- Terminate TLS at the edge and pin internal certificates.
- Keep management planes on a separate network segment.

## Logging

- Ship audit logs to the central collector within five minutes.
- Alert on repeated authorization failures.
- Retain access logs for at least 180 days.

*This page is served from https://docs.northwind-labs.example/docs/security-hardening.*
