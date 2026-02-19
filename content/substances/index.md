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
- Nullable: **`false`**

### CasRn

- type: **`<string>`**
- Nullable: **`false`**

### GreenScreen

- type: **`<string>`**
- Nullable: **`false`**

### Min

- type: **`<int>`**
- Nullable: **`false`**

### Max

- type: **`<int>`**
- Nullable: **`true`**

### Residual

- type: **`<string>`**
- Nullable: **`false`**

### Recycle

- type: **`<string>`**
- Nullable: **`false`**

### AlternateOf

- type: **`<object>`**
- Nullable: **`true`**
- related: [Substance](./#app)
- default: **`null|string`**

::: warning CAUTION
Alternates for `Substances` is now a references to a `primary` instance of their respective objects.
:::

### Nano

- type: **`<string>`**
- Nullable: **`false`**

### Role

- type: **`<string>`**
- Nullable: **`false`**

### Notes

- type: **`<string>`**
- Nullable: **`true`**
- default: **`string`**

### ScreenedAt

- type: **`<string>`**
- Nullable: **`false`**

### Hazards

- type: **`<array>`**
- Nullable: **`true`**
- related: [Hazards](./hazards)
- default: **`string`**

### Listings

- type: **`<array>`**
- Nullable: **`true`**
- related: [Listings](./listings)
- default: **`string`**
