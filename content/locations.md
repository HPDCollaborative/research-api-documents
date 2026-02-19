---
title: Locations
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> Locations are an addition to the 2.3 Standard.

## Structure

Locations are `implemented` as a Social Equity Indicator and apply to [Nested Materials](nested-materials/), [Substances](substances/), [Materials](materials/) and [Polymers](polymers).

```json
[
  {
    "Country": "<string>",
    "Latitude": "<decimal:10,7|string>" ,
    "Longitude": "<decimal:10,7|string>" ,
    "Stage": "<string>",
  }
]
```


### Country

- type: **`<string>`**
- Nullable: **`false`**

### Latitude

- type: **`<decimal:10,7|string>`**
- Nullable: **`true`**
- default: **`<null|string>`**

### Longitude

- type: **`<decimal:10,7|string>`**
- Nullable: **`true`**
- default: **`<null|string>`**

### Stage

- type: **`<string>`**
- Nullable: **`false`**