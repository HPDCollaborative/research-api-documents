---
title: Metal Alloys
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
	"MetalAlloy": {
		"UnsOrEnIdentifier": "<string>",
		"MetalAlloyHpd": "<string>",
		"GreenScreenAlloyingElements": "<string>",
		"ListingNotes": "<string>"
	}
}
```

#### DIFF 2.2 > 2.3

```diff
+ "MetalAlloy": {
+   "UnsOrEnIdentifier": "<string>",
+   "MetalAlloyHpd": "<string>",
+   "GreenScreenAlloyingElements": "<string>",
+   "ListingNotes": "<string>"
+ }
```

### UnsOrEnIdentifier

- type: **`<string>`**
- required: **`true`**

### MetalAlloyHpd

- type: **`<string>`**
- required: **`true`**

### GreenScreenAlloyingElements

- type: **`<string>`**
- required: **`true`**

### ListingNotes

- type: **`<string>`**
- required: **`true`**
