---
title: Hazards
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

Hazards, if included, exist as an array of Hazard objects listed with the key of `Hazards` and are structured as follows:

```json
[ // Start of "Hazards" array
  {
    "Name": "<string>",
    "List": "<string>",
    "Endpoint": "<string>",
    "Abbreviation": "<string>"
  }
  ...
]
```

### Name

- type: **`<string>`**
- required: **`true`**

### List

- type: **`<string>`**
- required: **`true`**

### Endpoint

- type: **`<string>`**
- required: **`true`**

### Abbreviation

- type: **`<string>`**
- required: **`true`**
