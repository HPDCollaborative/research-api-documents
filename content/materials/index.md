---
title: Materials
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

::: info
Material is a refactored object from v2.2, for what is now a `Nested Material` in v2.3 of the Standard. Materials were previously part of Substances and known as `Special Conditions`.
:::

## Structure

Materials exist as an array of Material objects listed with the key of `Materials` and are structured as follows:

```json
[ // Start of "Materials" array
  {
    "Name": "<string>",
    "Condition": "<object>",
    "Min": "<float>",
    "Max": "<float>",
    "AlternateOf": "<object>",
    "Recycle": "<string>",
    "Nano": "<bool>",
    "Role": "<string>",
    "Notes": "<string>",
    "Locations": "<decimal:10,7|string>"
  }
  ...
]
```

### Name

- type: **`<string>`**
- Nullable: **`false`**

### Condition

- type: **`<object>`**
- Nullable: **`false`**
- related: 1 of 6 Special Conditions
  - [Biological](./biological)
  - [Geological](./geological)
  - [Mixed Content](./mixed-content)
  - [Electronics](./electronics)
  - [Fasteners](./fasteners)
  - [Metal Alloys](./metal-alloys)

### Min

- type: **`<float>`**
- Nullable: **`false`**

### Max

- type: **`<float>`**
- Nullable: **`true`**

### AlternateOf

- type: **`<object>`**
- Nullable: **`true`**
- related: [Material](./#app)
- default: **`null|string`**

::: warning CAUTION
`AlternateOf` for a `Materials` is now a reference to a `primary` Material within the same `Nested Material`.
:::

### Recycle

- type: **`<string>`**
- Nullable: **`false`**

### Nano

- type: **`<bool>`**
- Nullable: **`false`**

### Role

- type: **`<string>`**
- Nullable: **`false`**

### Notes

- type: **`<string>`**
- Nullable: **`true`**

### Locations

- type: **`array`**
- Nullable: **`true`**
- related: [Locations](../locations)
- default: **`string`**