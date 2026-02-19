---
title: Listings
category: Content
---

# {{ $frontmatter.title }}

::: info
Listings is a new data array that represents Additional Hazard Listings.
:::

[[toc]]

## Structure

```json
[
  {
    "Listing": "<string>",
    "Agency": "<string>",
    "Notification": "<string>"
  }
  ...
]
```

---

### Listing

- type: **`<string>`**
- Nullable: **`false`**

### Agency

- type: **`<string>`**
- Nullable: **`false`**

### Notification

- type: **`<string>`**
- Nullable: **`false`**
