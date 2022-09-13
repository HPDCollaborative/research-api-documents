---
title: Materials
lastUpdated: true
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
[
  {
    "Name": "<string>",
    "Condition": "<object>",
    "Min": "<float>",
    "Max": "<float>",
    "AlternateOf": "<object>",
    "Recycle": "<string>",
    "Nano": "<bool>",
    "Role": "<string>",
    "Notes": "<string>"
  }
  ...
]
```

#### DIFF 2.2 > 2.3

```diff
+ "Condition": "<object>"
+ "AlternateOf": "<object>"
- "Alternate": "<string>"
- "Reportable": "<string>"
- "HpdUrl": "<string>"
- "Threshold": "<string>"
- "Residuals": "<string>"
- "ResidualNotes": "<string>"
- "MaterialType": "<string>"
- "Substances": "<string>"
```

### Name

- type: **`<string>`**
- required: **`true`**

### Condition

- type: **`<object>`**
- required: **`true`**
- related: 1 of 6 Special Conditions
  - [Biological](./special-conditions/biological.md)
  - [Geological](./special-conditions/geological.md)
  - [Mixed Content](./special-conditions/geological.md)
  - [Electronics](./special-conditions/geological.md)
  - [Fasteners](./special-conditions/geological.md)
  - [Metal Alloys](./special-conditions/geological.md)

### Min

- type: **`<float>`**
- required: **`true`**

### Max

- type: **`<float>`**
- required: **`false`**

### AlternateOf

- type: **`<object>`**
- required: **`false`**
- related: [Material](./#app)
- default: **`null|string`**

::: warning CAUTION
Alternates for `Materials` are now references to a `primary` or `parent` instance of their respective objects.
:::

### Recycle

- type: **`<string>`**
- required: **`true`**

### Nano

- type: **`<bool>`**
- required: **`true`**

### Role

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`false`**
