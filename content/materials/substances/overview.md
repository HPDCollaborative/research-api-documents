---
title: Substances
category: Content
---

# {{ $frontmatter.title }} {.doc-heading}

[[toc]]

## Structure {.doc-heading}

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

### Name {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### CasRn {.doc-heading}

- type: **`<string>`**
- required: **`false`**

### GreenScreen {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Payload {.doc-heading}

- type: **`<array>`**
- required: **`false`**

### Min {.doc-heading}

- type: **`<float>`**
- required: **`true`**

### Max {.doc-heading}

- type: **`<float>`**
- required: **`true`**

### Name {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Residual {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Recycle {.doc-heading}

- type: **`<bool>`**
- required: **`true`**

### Nano {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Role {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Notes {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### ScreenedAt {.doc-heading}

- type: **`<timestamp>`**
- required: **`true`**

### Hazards {.doc-heading}

- type: **`<array>`**
- required: **`false`**
- related: [Hazards](./hazards)
