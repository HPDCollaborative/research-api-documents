---
title: Materials
category: Content
---

# {{ $frontmatter.title }} {.doc-heading}

[[toc]]

## Structure {.doc-heading}

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

### Name {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Min {.doc-heading}

- type: **`<float>`**
- required: **`true`**

### Max {.doc-heading}

- type: **`<float>`**
- required: **`true`**

### Alternate {.doc-heading}

- type: **`<bool>`**
- required: **`true`**

### Reportable {.doc-heading}

- type: **`<bool>`**
- required: **`true`**

### HpdUrl {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Threshold {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Residuals {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### ResidualNotes {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Notes {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### MaterialType {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Substances {.doc-heading}

- type: **`<string>`**
- required: **`true`**
- related: [Substances](./substances/)
