---
title: Mixed Recycled Content
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
	"MixedRecycledContent": {
		"IngredientDescription": "<string>",
		"TestingPerformed": "<string>",
		"TestingDescription": "<string>",
		"BatchVariation": "<string>",
		"VariationDescription": "<string>",
		"CountryOfOrigin": "<string>",
		"MissingInformation": "<string>"
	}
}
```

#### DIFF 2.2 > 2.3

```diff
+ "MixedRecycledContent": {
+   "IngredientDescription": "<string>",
+   "TestingPerformed": "<string>",
+   "TestingDescription": "<string>",
+   "BatchVariation": "<string>",
+   "VariationDescription": "<string>",
+   "CountryOfOrigin": "<string>",
+   "MissingInformation": "<string>"
+ }
```

### IngredientDescription

- type: **`<string>`**
- required: **`true`**

### TestingPerformed

- type: **`<string>`**
- required: **`true`**

### TestingDescription

- type: **`<string>`**
- required: **`true`**

### BatchVariation

- type: **`<string>`**
- required: **`true`**

### VariationDescription

- type: **`<string>`**
- required: **`true`**

### CountryOfOrigin

- type: **`<string>`**
- required: **`true`**

### MissingInformation

- type: **`<string>`**
- required: **`true`**
