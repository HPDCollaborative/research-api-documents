---
title: Substances
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
[
  {
    "Name": "<string>",
    "CasRn": "<string>",
    "GreenScreen": "<string>",
    "Payload": "<array>",
    "Min": "<float>",
    "Max": "<float>",
    "Residual": "<string>",
    "Recycle": "<bool>",
    "Nano": "<bool>",
    "Role": "<string>",
    "Notes": "<string>",
    "ScreenedAt": "<string>",
    "Hazards": "<array>"
  }
]
```

### Name

- type: **`<string>`**
- required: **`true`**

### CasRn

- type: **`<string>`**
- required: **`false`**

### GreenScreen

- type: **`<string>`**
- required: **`true`**

### Payload

- type: **`<array>`**
- required: **`false`**

### Min

- type: **`<float>`**
- required: **`true`**

### Max

- type: **`<float>`**
- required: **`true`**

### Name

- type: **`<string>`**
- required: **`true`**

### Residual

- type: **`<string>`**
- required: **`true`**

### Recycle

- type: **`<bool>`**
- required: **`true`**

### Nano

- type: **`<string>`**
- required: **`true`**

### Role

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`true`**

### ScreenedAt

- type: **`<timestamp>`**
- required: **`true`**

### Hazards

- type: **`<array>`**
- required: **`false`**
- related: [Hazards](./hazards)
