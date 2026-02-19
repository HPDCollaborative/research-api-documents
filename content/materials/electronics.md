---
title: Electronics Material
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> `{{ $frontmatter.title }}` is an addition to the 2.3 Standard.

## Structure

`{{ $frontmatter.title }}` is an object that can be attached to a [Material](../materials/) object under the `Condition` key.

```json
{
  "ElectronicComponent": {
    "IngredientDescription": "<string>",
    "Compliance": "<string>",
    "ComplianceExemptions": "<string>",
    "Takeback": "<string>",
    "OtherEolExplanation": "<string>"
  }
}
```

### IngredientDescription

- type: **`<string>`**
- Nullable: **`false`**

### Compliance

- type: **`<string>`**
- Nullable: **`false`**

### ComplianceExemptions

- type: **`<string>`**
- Nullable: **`false`**

### Takeback

- type: **`<string>`**
- Nullable: **`false`**

### OtherEolExplanation

- type: **`<string>`**
- Nullable: **`false`**