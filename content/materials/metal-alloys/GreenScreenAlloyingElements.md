---
title:GreenScreen Alloying Elements
category: Metal Alloys
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> `{{ $frontmatter.title }}` is an object that can be attached to a [Metal Alloy](../metal-alloys/) object.

## Structure

```json

{
    "Name": "<string>",
    "Casrn": "<string>",
    "Percentage": {
        "min_per_percentage": "<string>",
        "max_per_percentage": "<string>"
    },
    "ElementRole": "<string>",
    "GreenScreenScore": "<string>",
    "Listings":[
        "<string>"
    ]
}

```

### Name

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### Casrn

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**    

### Percentage

- type: **`json`**
```json
{
    "min_per_percentage": "<string>",
    "max_per_percentage": "<string>"
}
```
- required: **`false`**
- default: **`null|object`**

### ElementRole

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### GreenScreenScore

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### Listings

- type: **`<array>`**
- required: **`false`**
- default: **`null|array`**
