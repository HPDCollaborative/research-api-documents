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
- Nullable: **`false`**

### MetalAlloyHpd

- type: **`<string>`**
- Nullable: **`false`**

### GreenScreenAlloyingElements

- type: **`<array>`**
- Nullable: **`true`**
- related: [GreenScreenAlloyingElements](./GreenScreenAlloyingElements)

### ListingNotes

- type: **`<string>`**
- Nullable: **`false`**

### IsAssociated

- type: **`<string>`**
- Nullable: **`false`**

### IsPotableWater

- type: **`<string>`**
- Nullable: **`false`**
