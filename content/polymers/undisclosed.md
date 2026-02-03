---
title: Polymer - Unwilling to Share
category: content
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> `{{ $frontmatter.title }}` is an addition to the 2.3 Standard.

## Structure

`{{ $frontmatter.title }}` is a variation of [Polymers](../polymers/) and will be found within the `Polymers` array.

```json
[ // Start "Polymers" array
  {
    "Name": "<string>",
    "Identifier": "<string>",
    "GreenScreen": "<string>",
    "ScreeningEngine": "<string>",
    "Min": "<float>",
    "Max": "<float>",
    "Residual": "<string>",
    "Recycle": "<string>",
    "AlternateOf": "<object|string>",
    "Nano": "<string>",
    "Role": "<string>",
    "PolymerType": "<string>",
    "AverageMolecularWeight": "<string>",
    "PercentOfMolecularWeightLessThan500Da": "<string>",
    "AdditionalSubstancesConsidered": "<string|null>",
    "GHSHazardStatements": "<string>",
    "HazardScreeningCompliance": "<string>",
    "PolymerNotes": "<string>",
    "AdditionalNotes": "<string>",
    "ScreenedAt": "<string>",
    "Locations": "<array>",
  }
  ...
]
```

#### DIFF 2.2 > 2.3

```diff
+ "Polymers": {
+   "Name": "<string>",
+   "Identifier": "<string>",
+   "GreenScreen": "<string>",
+   "ScreeningEngine": "<string>",
+   "Min": "<float>",
+   "Max": "<float>",
+   "Residual": "<string>",
+   "Recycle": "<string>",
+   "AlternateOf": "<object|string>",
+   "Nano": "<string>",
+   "Role": "<string>",
+   "PolymerType": "<string>",
+   "AverageMolecularWeight": "<string>",
+   "PercentOfMolecularWeightLessThan500Da": "<string>",
+   "AdditionalSubstancesConsidered": "<string|null>",
+   "GHSHazardStatements": "<string>",
+   "HazardScreeningCompliance": "<string>",
+   "PolymerNotes": "<string>",
+   "AdditionalNotes": "<string>",
+   "ScreenedAt": "<string>",
+   "Locations": "<array>",
+ }
```

### Name

- type: **`<string>`**
- required: **`true`**
- default: **`Undisclosed`**

::: danger CAUTION
This will always return Undisclosed
:::

### Identifier

- type: **`<string>`**
- required: **`true`**
- default: **`Undisclosed`**

::: danger CAUTION
This will always return Undisclosed
:::

### GreenScreen

- type: **`<string>`**
- required: **`true`**

### ScreeningEngine

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
- related: [Polymer](./)
- default: **`null|string`**

::: warning CAUTION
`AlternateOf` for a `Polymer` is now a reference to a `primary` Polymer within the same `NestedMaterial`.
:::

### Nano

- type: **`<string>`**
- required: **`true`**

### Role

- type: **`<string>`**
- required: **`true`**

### PolymerType

- type: **`<string>`**
- required: **`true`**

### AverageMolecularWeight

- type: **`<string>`**
- required: **`true`**

### PercentOfMolecularWeightLessThan500Da

- type: **`<string>`**
- required: **`true`**

### AdditionalSubstancesConsidered

- type: **`<string>`**
- required: **`true`**

### GHSHazardStatements

- type: **`<string>`**
- required: **`true`**

### HazardScreeningCompliance

- type: **`<string>`**
- required: **`true`**

### PolymerNotes

- type: **`<string>`**
- required: **`true`**

### AdditionalNotes

- type: **`<string>`**
- required: **`false`**
- default: **`string`**

### ScreenedAt

- type: **`<string>`**
- required: **`true`**

### Locations

- type: **`array`**
- required: **`false`**
- related: [Locations](../locations)
- default: **`string`**
