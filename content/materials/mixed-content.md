---
title: Mixed Recycled Content Material
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



### IngredientDescription

- type: **`<string>`**
- Nullable: **`false`**

### TestingPerformed

- type: **`<string>`**
- Nullable: **`false`**

### TestingDescription

- type: **`<string>`**
- Nullable: **`false`**

### BatchVariation

- type: **`<string>`**
- Nullable: **`false`**

### VariationDescription

- type: **`<string>`**
- Nullable: **`false`**

### CountryOfOrigin

- type: **`<string>`**
- Nullable: **`false`**

### MissingInformation

- type: **`<string>`**
- Nullable: **`false`**