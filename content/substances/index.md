---
title: Substances
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

Substances, if included, exist as an array of Substance objects listed with the key of `Substances` and are structured as follows:

```json
[ // Start of "Substances" array
  {
    "Name": "<string>",
    "CasRn": "<string>",
    "GreenScreen": "<string>",
    "ScreeningEngine": "<string>",
    "Min": "<float>",
    "Max": "<float>",
    "Residual": "<string>",
    "Recycle": "<string>",
    "AlternateOf": "<object|string>",
    "Nano": "<bool>",
    "Role": "<string>",
    "Notes": "<string>",
    "ScreenedAt": "<timestamp>",
    "Hazards": "<array>",
    "Listings": "<array>",
    "Locations": "<array>"
  },
  ...
]
```

#### DIFF 2.2 > 2.3

```diff
- "Payload": "<array>"
- "Residual": "<bool>"
+ "ScreeningEngine": "<string>",
+ "AlternateOf": "<object|string>"
+ "Residual": "<string>"
+ "Listings": "<array>"
+ "Locations": "<array>"
```

### Name

- type: **`<string>`**
- required: **`true`**

### CasRn

- type: **`<string>`**
- required: **`true`**

### GreenScreen

- type: **`<string>`**
- required: **`true`**

### Min

- type: **`<float>`**
- required: **`true`**

### Max

- type: **`<float>`**
- required: **`false`**

### Residual

- type: **`<string>`**
- required: **`true`**

### Recycle

- type: **`<string>`**
- required: **`true`**

### AlternateOf

- type: **`<object>`**
- required: **`false`**
- related: [Substance](./#app)
- default: **`null|string`**

::: warning CAUTION
`AlternateOf` for a `Substance` is now a reference to a `primary` Substance within the same `NestedMaterial`.
:::

### Nano

- type: **`<string>`**
- required: **`true`**

### Role

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`false`**
- default: **`string`**

### ScreenedAt

- type: **`<string>`**
- required: **`true`**

### Hazards

- type: **`<array>`**
- required: **`false`**
- related: [Hazards](./hazards)
- default: **`string`**

### Listings

- type: **`<array>`**
- required: **`false`**
- related: [Listings](./listings)
- default: **`string`**

### Locations

- type: **`array`**
- required: **`false`**
- related: [Locations](../locations)
- default: **`string`**
