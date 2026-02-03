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
```

#### DIFF 2.2 > 2.3

```diff
+ "NestedMaterials": [
+   {
+     "Name": "<string>",
+     "Min": "<float>",
+     "Max": "<float>",
+     "AlternateOf": "<object>",
+     "NoReportableSubstances": "<bool>",
+     "Threshold": "<int>",
+     "Residuals": "<string>",
+     "Notes": "<string>",
+     "ResidualNotes": "<string>",
+     "MaterialType": "<string>",
+     "Substances": "<array|string>",
+     "Materials": "<array|string>",
+     "Polymers": "<array|string>",
+     "Locations": "<array|string>"
+   }
+ ]
```

### Name

- type: **`<string>`**
- required: **`true`**

### Min

- type: **`<float>`**
- required: **`true`**

### Max

- type: **`<float>`**
- required: **`false`**

### AlternateOf

- type: **`<object>`**
- required: **`false`**
- related: [NestedMaterial](./#app)
- default: **`null|string`**

::: warning CAUTION
`AlternateOf` for a `Nested Material` is now a reference to a `primary` Nested Material within the same `Record`.
:::

### NoReportableSubstances

- type: **`<string>`**
- required: **`true`**

### Threshold

- type: **`<string>`**
- required: **`true`**

### Residuals

- type: **`<string>`**
- required: **`true`**

### ResidualNotes

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`true`**

### MaterialType

- type: **`<string>`**
- required: **`true`**

### Substances

- type: **`array`**
- required: **`false`**
- related: [Substances](../substances/)
- default: **`string`**

### Materials

- type: **`array`**
- required: **`false`**
- related: [Materials](../materials/)
- default: **`string`**

### Polymers

- type: **`array`**
- required: **`false`**
- related: [Polymers](../polymers/)
- default: **`string`**

::: danger
Even though `Substances`, `Materials` and `Polymers` are marked as "not required" above, make sure you receive at least 1 of either. If none are present and the `NoReportableSubstances` prop is `No`, this is not a valid HPD.
:::

### Locations

- type: **`array`**
- required: **`false`**
- related: [Locations](../locations)
- default: **`string`**