---
title: Geological Material
lastUpdated: true
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "Origin": "<string>",
  "IngredientComposition": "<string>",
  "PotentialPresenceOfToxicMaterials": "<string>",
  "ToxicMaterialDescription": "<string>",
  "PresenceOfRadioactiveElements": "<string>",
  "RadioactiveElementDescription": "<string>"
}
```

#### DIFF 2.2 > 2.3

```diff
+   "Origin": "<string>"
+   "IngredientComposition": "<string>"
+   "PotentialPresenceOfToxicMaterials": "<string>"
+   "ToxicMaterialDescription": "<string>"
+   "PresenceOfRadioactiveElements": "<string>"
+   "RadioactiveElementDescription": "<string>"
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
