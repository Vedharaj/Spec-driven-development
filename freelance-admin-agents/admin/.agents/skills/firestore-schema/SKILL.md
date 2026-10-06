# Firestore Schema

## Principles

Use collections based on business entities.

Example:

/projects
/services
/testimonials
/pages
/settings
/users

## Document Rules

Every mutable document should normally contain:

- id
- createdAt
- updatedAt

Content that requires publishing should also contain:

- published
- publishedAt

Ordered content should contain:

- order

## Example Project

```text
projects/{projectId}

{
  title,
  slug,
  shortDescription,
  description,
  highlight,

  category,
  technologies,

  coverImage,
  gallery,

  projectUrl,
  githubUrl,

  featured,
  published,
  order,

  seo: {
    title,
    description,
    image
  },

  createdAt,
  updatedAt,
  publishedAt
}
```
