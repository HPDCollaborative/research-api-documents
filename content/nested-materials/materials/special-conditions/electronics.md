---
title: Electronics
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

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
