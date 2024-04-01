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
