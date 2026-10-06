# Image Management

## Purpose

Manage images used by the public website.

## Workflow

Select file
→ Validate
→ Upload to Firebase Storage
→ Obtain Storage reference/URL
→ Save metadata in Firestore
→ Display in admin
→ Display on public site

## Validation

Check:
- MIME type
- extension
- file size
- image dimensions when relevant

## Rules

Do not put image binaries in Firestore.
