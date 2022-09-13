---
title: Nested Materials
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

::: danger IMPORTANT
Nested Materials is a new data array that supercedes Materials in version 2.2 and earlier.
:::

[[toc]]

## Structure

```json
{
  "Name": "<string>",
  "Min": "<float>",
  "Max": "<float>",
  "AlternateOf": "<object>",
  "NoReportableSubstances": "<bool>",
  "Threshold": "<int>",
  "Residuals": "<string>",
  "ResidualNotes": "<string>",
  "MaterialType": "<string>",
  "Substances": "<array>",
  "Materials": "<array>"
}
```

#### DIFF 2.2 > 2.3

```diff
+ "Name": "<string>"
+ "Min": "<float>"
+ "Max": "<float>"
+ "AlternateOf": "<object>"
+ "NoReportableSubstances": "<bool>"
+ "Threshold": "<int>"
+ "Residuals": "<string>"
+ "ResidualNotes": "<string>"
+ "MaterialType": "<string>"
+ "Substances": "<array>"
+ "Materials": "<array>"
```

---

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
Alternate for `Nested Materials`is now a reference to a `primary` instance of their respective objects.
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

### MaterialType

- type: **`<string>`**
- required: **`true`**

### Substances

- type: **`array`**
- required: **`false`**
- related: [Substances](./substances/)
- default: **`string`**

### Materials

- type: **`array`**
- required: **`false`**
- related: [Materials](./materials/)
- default: **`string`**

::: danger
Even though both `Materials` and `Substances` are marked as "not required" above, make sure you receive at least 1 of either. If neither are present and the `NoReportableSubstances` prop is `No`, this is not a valid HPD.
:::
