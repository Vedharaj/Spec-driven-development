# Firebase Storage

## Purpose

Manage website media without storing binary data in Firestore.

## Suggested Structure

```text
site/
  projects/
  services/
  testimonials/
  pages/
  branding/

admin/
  temporary/
```

## Rules

Every upload should validate:
- MIME type
- extension
- file size

Store image metadata and Storage references in Firestore.

Do not store binary image data directly inside Firestore documents.

Use predictable paths and prevent unauthorized file access.
