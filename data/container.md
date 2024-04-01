---
title: Data Container
category: Data
---

# {{ $frontmatter.title }} {.doc-heading}

[[toc]]

## Structure {.doc-heading}

The base data object should return the following JSON structure.

```json
{
  "NumericId": "<int>",
  "DigitalId": "<string>",
  "RecordId": "<int>",
  "Build": "<string>",
  "FileName": "<string>",
  "Accessories": "<array>",
  "Certifications": "<array>",
  "Company": "<object>",
  "Content": "<object>",
  "General": "<object>",
  "Notes": "<object>",
  "Parts": "<array>",
  "Product": "<object>",
  "Reference": "<object>",
  "Voc": "<object>",
  "PublishedAt": "<timestamp>",
  "WithdrawnAt": "<timestamp>",
  "ScreenedAt": "<timestamp>"
}
```

### NumericId {.doc-heading}

- type: **`<int>`**
- required: **`true`**

### DigitalId {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### RecordId {.doc-heading}

- type: **`<int>`**
- required: **`true`**

### Build {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Filename {.doc-heading}

- type: **`<string>`**
- required: **`true`**

### Accessories {.doc-heading}

- type: **`<array>`**
- required: **`false`**
- related: [Accessories](./accessories)
- default: **`null|string`**

### Certifications {.doc-heading}

- type: **`<array>`**
- required: **`true`**
- related: [Certifications](./certifications)

### Company {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [Company](./company)

### Content {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [Content](../content/)

::: info
The content prop is simply a JSON object that wraps an HPD's content inventory. Content inventory details and structure, are documented in the [Content Inventory section](../content/) below.
:::

### General {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [General](./general)

::: tip
The data object represents the Summary section of the HPD.
:::

### Notes {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [Notes](./notes)

### Parts {.doc-heading}

- type: **`<array>`**
- required: **`false`**
- related: [Parts](./parts)
- default: **`null`**

### Product {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [Product](./product)

### Reference {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [Reference](./reference)

### Voc {.doc-heading}

- type: **`<object>`**
- required: **`true`**
- related: [VOC](./voc)

### PublishedAt {.doc-heading}

- type: **`<timestamp>`**
- required: **`true`**

### WithdrawnAt {.doc-heading}

- type: **`<timestamp>`**
- required: **`false`**
- default: **`null`**

### ScreenedAt {.doc-heading}

- type: **`<timestamp>`**
- required: **`true`**
