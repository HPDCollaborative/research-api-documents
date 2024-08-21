---
title: Metal Alloys Material
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
