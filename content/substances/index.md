---
title: Substances
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "Name": "<string>",
  "CasRn": "<string>",
  "GreenScreen": "<string>",
  "Min": "<float>",
  "Max": "<float>",
  "Residual": "<string>",
  "Recycle": "<string>",
  "AlternateOf": "<object>",
  "Nano": "<bool>",
  "Role": "<string>",
  "Notes": "<string>",
  "ScreenedAt": "<timestamp>",
  "Hazards": "<array>",
  "Listings": "<array>"
}
```


---

### Name

- type: **`<string>`**
- required: **`true`**

### CasRn

- type: **`<string>`**
- required: **`true`**

### GreenScreen

- type: **`<string>`**
- required: **`true`**

### Min

- type: **`<int>`**
- required: **`true`**

### Max

- type: **`<int>`**
- required: **`false`**

### Residual

- type: **`<string>`**
- required: **`true`**

### Recycle

- type: **`<string>`**
- required: **`true`**

### AlternateOf

- type: **`<object>`**
- required: **`false`**
- related: [Substance](./#app)
- default: **`null|string`**

::: warning CAUTION
Alternates for `Substances` is now a references to a `primary` instance of their respective objects.
:::

### Nano

- type: **`<string>`**
- required: **`true`**

### Role

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`false`**
- default: **`string`**

### ScreenedAt

- type: **`<string>`**
- required: **`true`**

### Hazards

- type: **`<array>`**
- required: **`false`**
- related: [Hazards](./hazards)
- default: **`string`**

### Listings

- type: **`<array>`**
- required: **`false`**
- related: [Listings](./listings)
- default: **`string`**
