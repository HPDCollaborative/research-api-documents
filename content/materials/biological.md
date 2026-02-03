---
title: Biological Material
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
  "BiologicalMaterial": {
    "Category": "<string>",
    "IngredientDescription": "<string>"
  }
}
```

#### DIFF 2.2 > 2.3

```diff
+ "BiologicalMaterial": {
+   "Category": "<string>",
+   "IngredientDescription": "<string>"
+ }
```

### Category

- type: **`<string>`**
- required: **`true`**

### IngredientDescription

- type: **`<string>`**
- required: **`true`**