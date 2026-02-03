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

#### DIFF 2.2 > 2.3

```diff
+ "GeologicalMaterial": {
+   "Origin": "<string>",
+   "IngredientComposition": "<string>",
+   "PotentialPresenceOfToxicMaterials": "<string>",
+   "ToxicMaterialDescription": "<string>",
+   "PresenceOfRadioactiveElements": "<string>",
+   "RadioactiveElementDescription": "<string>"
+ }
```

### Origin

- type: **`<string>`**
- required: **`true`**

### IngredientComposition

- type: **`<string>`**
- required: **`true`**

### PotentialPresenceOfToxicMaterials

- type: **`<string>`**
- required: **`true`**

### ToxicMaterialDescription

- type: **`<string>`**
- required: **`true`**

### PresenceOfRadioactiveElements

- type: **`<string>`**
- required: **`true`**

### RadioactiveElementDescription

- type: **`<string>`**
- required: **`true`**