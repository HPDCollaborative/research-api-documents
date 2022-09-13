---
title: Biological Material
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "Category": "<string>",
  "IngredientDescription": "<string>"
}
```

#### DIFF 2.2 > 2.3

```diff
+   "Category": "<string>"
+   "IngredientDescription": "<string>"
```

### Category

- type: **`<string>`**
- required: **`true`**

### IngredientDescription

- type: **`<string>`**
- required: **`true`**
