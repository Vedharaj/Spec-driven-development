# Firebase Integration

## Purpose

Provide a consistent integration approach for the shared Firebase project.

## Services

- Firebase Authentication
- Cloud Firestore
- Firebase Storage

## Rules

Use environment variables for client configuration.

Never expose service-account credentials.

Keep Firebase initialization centralized.

Keep Firestore and Storage access behind typed service modules.

Validate writes before persistence.

Document any required indexes and security rules.

## Architecture

PUBLIC_SITE:
- primarily reads published content.

ADMIN_SITE:
- authenticates administrators.
- performs authorized content operations.
