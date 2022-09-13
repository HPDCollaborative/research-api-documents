---
title: Data Container
lastUpdated: true
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

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

### NumericId

- type: **`<int>`**
- required: **`true`**

### DigitalId

- type: **`<string>`**
- required: **`true`**

### RecordId

- type: **`<int>`**
- required: **`true`**

### Build

- type: **`<string>`**
- required: **`true`**

### Filename

- type: **`<string>`**
- required: **`true`**

### Accessories

- type: **`<array>`**
- required: **`false`**
- related: [Accessories](./accessories)
- default: **`null|string`**

### Certifications

- type: **`<array>`**
- required: **`true`**
- related: [Certifications](./certifications)

### Company

- type: **`<object>`**
- required: **`true`**
- related: [Company](./company)

### Content

- type: **`<object>`**
- required: **`true`**
- related: [Content](../content/)

::: info
The content prop is simply a JSON object that wraps an HPD's content inventory. Content inventory details and structure, are documented in the [Content Inventory section](../content/) below.
:::

### General

- type: **`<object>`**
- required: **`true`**
- related: [General](./general)

::: tip
The data object represents the Summary section of the HPD.
:::

### Notes

- type: **`<object>`**
- required: **`true`**
- related: [Notes](./notes)

### Parts

- type: **`<array>`**
- required: **`false`**
- related: [Parts](./parts)
- default: **`null`**

### Product

- type: **`<object>`**
- required: **`true`**
- related: [Product](./product)

### Reference

- type: **`<object>`**
- required: **`true`**
- related: [Reference](./reference)

### Voc

- type: **`<object>`**
- required: **`true`**
- related: [VOC](./voc)

### PublishedAt

- type: **`<timestamp>`**
- required: **`true`**

### WithdrawnAt

- type: **`<timestamp>`**
- required: **`false`**
- default: **`null`**

### ScreenedAt

- type: **`<timestamp>`**
- required: **`true`**
