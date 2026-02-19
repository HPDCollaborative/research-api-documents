---
title: Nested Materials
category: Content
---

# {{ $frontmatter.title }}

::: danger IMPORTANT
Nested Materials is a new data array that supercedes Materials in version 2.2 and earlier.
:::

[[toc]]

## Structure

Nested Materials exist as an array of NestedMaterial objects listed with the key of `NestedMaterials` and are structured as follows:

```json
[ // Start of "NestedMaterials" array
  {
    "Name": "<string>",
    "Min": "<float>",
    "Max": "<float>",
    "AlternateOf": "<object|string>",
    "NoReportableSubstances": "<bool>",
    "Threshold": "<int>",
    "Residuals": "<string>",
    "ResidualNotes": "<string>",
    "Notes": "<string>",
    "MaterialType": "<string>",
    "Substances": "<array|string>",
    "Materials": "<array|string>",
    "Polymers": "<array|string>",
    "Locations": "<array|string>"
  },
  ...
]


### Name

- type: **`<string>`**
- Nullable: **`false`**

### Min

- type: **`<float>`**
- Nullable: **`false`**

### Max

- type: **`<float>`**
- Nullable: **`true`**

### AlternateOf

- type: **`<object>`**
- Nullable: **`true`**
- related: [NestedMaterial](./#app)
- default: **`null|string`**

::: warning CAUTION
`AlternateOf` for a `Nested Material` is now a reference to a `primary` Nested Material within the same `Record`.
:::

### NoReportableSubstances

- type: **`<string>`**
- Nullable: **`false`**

### Threshold

- type: **`<string>`**
- Nullable: **`false`**

### Residuals

- type: **`<string>`**
- Nullable: **`false`**

### ResidualNotes

- type: **`<string>`**
- Nullable: **`false`**

### Notes

- type: **`<string>`**
- Nullable: **`false`**

### MaterialType

- type: **`<string>`**
- Nullable: **`false`**

### Substances

- type: **`array`**
- Nullable: **`true`**
- related: [Substances](../substances/)
- default: **`string`**

### Materials

- type: **`array`**
- Nullable: **`true`**
- related: [Materials](../materials/)
- default: **`string`**

### Polymers

- type: **`array`**
- Nullable: **`true`**
- related: [Polymers](../polymers/)
- default: **`string`**

::: danger
Even though `Substances`, `Materials` and `Polymers` are marked as "not required" above, make sure you receive at least 1 of either. If none are present and the `NoReportableSubstances` prop is `No`, this is not a valid HPD.
:::

### Locations

- type: **`array`**
- Nullable: **`true`**
- related: [Locations](../locations)
- default: **`string`**