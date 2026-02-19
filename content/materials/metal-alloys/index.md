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
        "GreenScreenAlloyingElements": [
           "<object>"
        ],
        "ListingNotes": "<string>",
        "IsAssociated": "<string>",
        "IsPotableWater": "<string>"
    }
}
```

#### DIFF 2.3 > 3.0

```diff
+ "MetalAlloy": {
-   "GreenScreenAlloyingElements": "<string>",
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
- related: [GreenScreenAlloyingElements](./GreenScreenAlloyingElements)

### ListingNotes

- type: **`<string>`**
- required: **`true`**

### IsAssociated

- type: **`<string>`**
- required: **`true`**

### IsPotableWater

- type: **`<string>`**
- required: **`true`**
