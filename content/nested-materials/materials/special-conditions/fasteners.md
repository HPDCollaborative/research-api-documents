---
title: Fasteners
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
	"MinorFastener": {
		"ComponentComposition": "<string>",
		"EuRohsConformance": "<string>",
		"EuReachSvhcContent": "<string>",
		"EuRohsExemptions": "<string>",
		"SvhcDeclaration": "<string>",
		"LbcRedListCompliance": "<string>",
		"SpecialConditionThresholdDeclaration": "<string>"
	}
}
```

#### DIFF 2.2 > 2.3

```diff
+ "MinorFastener": {
+   "ComponentComposition": "<string>",
+   "EuRohsConformance": "<string>",
+   "EuReachSvhcContent": "<string>",
+   "EuRohsExemptions": "<string>",
+   "SvhcDeclaration": "<string>",
+   "LbcRedListCompliance": "<string>",
+   "SpecialConditionThresholdDeclaration": "<string>"
+ }
```

### ComponentComposition

- type: **`<string>`**
- required: **`true`**

### EuRohsConformance

- type: **`<string>`**
- required: **`true`**

### EuReachSvhcContent

- type: **`<string>`**
- required: **`true`**

### EuRohsExemptions

- type: **`<string>`**
- required: **`true`**

### SvhcDeclaration

- type: **`<string>`**
- required: **`true`**

### LbcRedListCompliance

- type: **`<string>`**
- required: **`true`**

### SpecialConditionThresholdDeclaration

- type: **`<string>`**
- required: **`true`**
