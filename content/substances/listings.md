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
- required: **`true`**

### Agency

- type: **`<string>`**
- required: **`true`**

### Notification

- type: **`<string>`**
- required: **`true`**
