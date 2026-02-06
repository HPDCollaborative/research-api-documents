---
title: Metal Alloys Material
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> `{{ $frontmatter.title }}` is an object that can be attached to a [Material](../materials/) object under the `Condition` key.

## Structure

```json
{
	"MetalAlloy": {
		"UnsOrEnIdentifier": "<string>",
		"MetalAlloyHpd": "<string>",
		"GreenScreenAlloyingElements": "<array>",
		"ListingNotes": "<string>",
		"IsAssociated": "<string>",
		"IsPotableWater": "<string>"
	}
}
```

#### DIFF 2.3 > 3.0

```diff
+ "MetalAlloy": {
+   "GreenScreenAlloyingElements": "<array>",
+   "IsAssociated": "<string>",
+	"IsPotableWater": "<string>"
+ }
```

### UnsOrEnIdentifier

- type: **`<string>`**
- required: **`true`**

### MetalAlloyHpd

- type: **`<string>`**
- required: **`true`**

### GreenScreenAlloyingElements

- type: **`<array>`**
- required: **`false`**
```json
{
	"GreenScreenAlloyingElements": [
		{
			"Name": "<string",
			"Casrn": "<string>",
			"Percentage": {
				"min_per_percentage": "<string",
				"max_per_percentage": "<string"
			},
			"Element Role": "<string>",
			"GreenScreen Score": "<string>",
			"Listings":[
				
			]
		}

	]
		
	
}
```
### ListingNotes

- type: **`<string>`**
- required: **`true`**
