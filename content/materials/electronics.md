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

#### DIFF 2.2 > 2.3

```diff
+ "ElectronicComponent": {
+   "IngredientDescription": "<string>",
+   "Compliance": "<string>",
+   "ComplianceExemptions": "<string>",
+   "Takeback": "<string>",
+   "OtherEolExplanation": "<string>"
+ }
```

### IngredientDescription

- type: **`<string>`**
- required: **`true`**

### Compliance

- type: **`<string>`**
- required: **`true`**

### ComplianceExemptions

- type: **`<string>`**
- required: **`true`**

### Takeback

- type: **`<string>`**
- required: **`true`**

### OtherEolExplanation

- type: **`<string>`**
- required: **`true`**