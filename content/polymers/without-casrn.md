---
title: Polymer without CASRN
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



### Name

- type: **`<string>`**
- Nullable: **`false`**

### Identifier

- type: **`<string>`**
- Nullable: **`false`**

### GreenScreen

- type: **`<string>`**
- Nullable: **`false`**

### ScreeningEngine

- type: **`<string>`**
- Nullable: **`false`**

### Min

- type: **`<float>`**
- Nullable: **`false`**

### Max

- type: **`<float>`**
- Nullable: **`true`**

### Residual

- type: **`<string>`**
- Nullable: **`false`**

### Recycle

- type: **`<string>`**
- Nullable: **`false`**

### AlternateOf

- type: **`<object>`**
- Nullable: **`true`**
- related: [Polymer](./)
- default: **`null|string`**

::: warning CAUTION
`AlternateOf` for a `Polymer` is now a reference to a `primary` Polymer within the same `NestedMaterial`.
:::

### Nano

- type: **`<string>`**
- Nullable: **`false`**

### Role

- type: **`<string>`**
- Nullable: **`false`**

### PolymerType

- type: **`<string>`**
- Nullable: **`false`**

### AverageMolecularWeight

- type: **`<string>`**
- Nullable: **`false`**

### PercentOfMolecularWeightLessThan500Da

- type: **`<string>`**
- Nullable: **`false`**

### AdditionalSubstancesConsidered

- type: **`<string>`**
- Nullable: **`false`**

### GHSHazardStatements

- type: **`<string>`**
- Nullable: **`false`**

### HazardScreeningCompliance

- type: **`<string>`**
- Nullable: **`false`**

### PolymerNotes

- type: **`<string>`**
- Nullable: **`false`**

### AdditionalNotes

- type: **`<string>`**
- Nullable: **`true`**
- default: **`string`**

### ScreenedAt

- type: **`<string>`**
- Nullable: **`false`**

### Locations

- type: **`array`**
- Nullable: **`true`**
- related: [Locations](../locations)
- default: **`string`**
