# Admin Authentication

## Purpose

Protect the standalone admin application.

## Requirements

- authenticated admin access
- protected routes
- logout
- session-aware UI
- unauthorized access handling
- server/trusted authorization checks where required

## Rules

Never use:
- localStorage-only roles
- hidden UI as authorization
- client-provided role fields as the security boundary

Authentication and authorization must be enforced by trusted backend/Firebase security mechanisms.
