# AGENTS.md

## Project

This repository contains a production public website and a separate administrative application.

The public website and admin application share Firebase services.

## Architecture

PUBLIC WEBSITE
→ Next.js

ADMIN PANEL
→ Next.js

BACKEND
→ Firebase Authentication
→ Cloud Firestore
→ Firebase Storage

## Development Philosophy

Use Spec-Driven Development.

Requirement
→ Analysis
→ Specification
→ Implementation
→ Validation

## Existing Website

The existing website is the source of truth for visual identity, content structure, information architecture, and user-facing behavior.

Read:
- DESIGN.md
- CONTENT.md
- ARCHITECTURE.md

before modifying the public website.

## Admin

Admin lives in /admin and must remain independently deployable.

## Firebase

Both applications use the same Firebase project.

Public website is primarily a consumer.
Admin is the content management application.

## Security

Never expose privileged credentials.
Never trust client authorization.
Protect administrative operations.

## Code Quality

Prefer:
- TypeScript
- reusable components
- typed Firebase services
- feature-based architecture
- validation
- error handling
- loading states
- empty states
- tests

Avoid:
- duplicated logic
- giant components
- unnecessary dependencies
- hardcoded business content
- unrelated refactoring

## Agent Workflow

Before coding:
1. Read relevant specification.
2. Read DESIGN.md.
3. Read ARCHITECTURE.md.
4. Understand affected files.
5. Implement the smallest correct change.
6. Test.
7. Review.

## Definition of Done

A feature is complete only when:
- specification satisfied
- implementation complete
- TypeScript passes
- lint passes
- functionality tested
- security reviewed where relevant
- public/admin integration verified
