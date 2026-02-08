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