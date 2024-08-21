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

#### DIFF 2.2 > 2.3

```diff
+ "Condition": "<object>"
+ "AlternateOf": "<object>"
+ "Locations": "<decimal:10,7|string>"
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
  - [Biological](./biological)
  - [Geological](./geological)
  - [Mixed Content](./mixed-content)
  - [Electronics](./electronics)
  - [Fasteners](./fasteners)
  - [Metal Alloys](./metal-alloys)

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
`AlternateOf` for a `Materials` is now a reference to a `primary` Material within the same `Nested Material`.
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

### Locations

- type: **`array`**
- required: **`false`**
- related: [Locations](../locations)
- default: **`string`**
