---
title: Geological Material
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
  "GeologicalMaterial": {
    "Origin": "<string>",
    "IngredientComposition": "<string>",
    "PotentialPresenceOfToxicMaterials": "<string>",
    "ToxicMaterialDescription": "<string>",
    "PresenceOfRadioactiveElements": "<string>",
    "RadioactiveElementDescription": "<string>"
  }
}
```


### Origin

- type: **`<string>`**
- Nullable: **`false`**

### IngredientComposition

- type: **`<string>`**
- Nullable: **`false`**

### PotentialPresenceOfToxicMaterials

- type: **`<string>`**
- Nullable: **`false`**

### ToxicMaterialDescription

- type: **`<string>`**
- Nullable: **`false`**

### PresenceOfRadioactiveElements

- type: **`<string>`**
- Nullable: **`false`**

### RadioactiveElementDescription

- type: **`<string>`**
- Nullable: **`false`**