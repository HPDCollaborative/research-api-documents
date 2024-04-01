---
title: Materials
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "Name": "<string>",
  "Min": "<float>",
  "Max": "<float>",
  "Alternate": "<string>",
  "Reportable": "<string>",
  "HpdUrl": "<string>",
  "Threshold": "<string>",
  "Residuals": "<string>",
  "ResidualNotes": "<string>",
  "Notes": "<string>",
  "MaterialType": "<string>",
  "Substances": "<string>"
}
```

### Name

- type: **`<string>`**
- required: **`true`**

### Min

- type: **`<float>`**
- required: **`true`**

### Max

- type: **`<float>`**
- required: **`true`**

### Alternate

- type: **`<bool>`**
- required: **`true`**

### Reportable

- type: **`<bool>`**
- required: **`true`**

### HpdUrl

- type: **`<string>`**
- required: **`true`**

### Threshold

- type: **`<string>`**
- required: **`true`**

### Residuals

- type: **`<string>`**
- required: **`true`**

### ResidualNotes

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`true`**

### MaterialType

- type: **`<string>`**
- required: **`true`**

### Substances

- type: **`<string>`**
- required: **`true`**
- related: [Substances](../substances/)
