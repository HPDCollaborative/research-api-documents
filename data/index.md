---
title: Data PDF
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

The base data object should return the following JSON structure.

```json
{
  "NumericId": "<string>",
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
  "PfasData": "<object>",
  "Product": "<object>",
  "Programs": "<object>",
  "Reference": "<object>",
  "UniqueProductId": "[<string>]",
  "Voc": "<object>",
  "PublishedAt": "<timestamp>",
  "WithdrawnAt": "<timestamp>",
  "ScreenedAt": "<timestamp>"
}
```
#### DIFF 2.3 > 3.0
```diff
+   "UniqueProductId": "[<string>]"
+   "PfasData": "<object>"
+   "Programs": "<object>"
```
### NumericId

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The unique identifier for the HPD, same as the UniqueId.`**

### DigitalId

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`GUID of the HPD`**

### RecordId

- type: **`<int>`**
- Nullable: **`false`**
- Definition: **`Record ID used on the Builder`**

### Build

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The version of the HPD Open Standard that the HPD was created with.`**

### Filename

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The name of the HPD file.`**

### Accessories

- type: **`<array>`**
- Nullable: **`true`**
- related: [Accessories](./accessories)

### Certifications

- type: **`<array>`**
- Nullable: **`false`**
- related: [Certifications](./certifications)

### Content

- type: **`<object>`**
- Nullable: **`false`**
- related: [Content](../content/)

::: info
The content prop is simply a JSON object that wraps an HPD's content inventory. Content inventory details and structure, are documented in the [Content Inventory section](../content/) below.
:::

### General 

- type: **`<object>`**
- Nullable: **`false`**
- related: [General](./general)

::: tip
The data object represents the Summary section of the HPD.
:::

### Notes

- type: **`<object>`**
- Nullable: **`false`**
- related: [Notes](./notes)

### Parts

- type: **`<array>`**
- Nullable: **`true`**
- related: [Parts](./parts)
- default: **`null`**

### PfasData

- type: **`<object>`**
- Nullable: **`true`**
- related: [PfasData](./pfasdata)
- default: **`null`**

### Product

- type: **`<object>`**
- Nullable: **`false`**
- related: [Product](./product)

### Programs

- type: **`<object>`**
- Nullable: **`true`**
- related: [Programs](./programs)

### Reference

- type: **`<object>`**
- Nullable: **`false`**
- related: [Reference](./reference)

### Voc

- type: **`<object>`**
- Nullable: **`false`**
- related: [VOC](./voc)

### PublishedAt

- type: **`<timestamp>`**
- Nullable: **`false`**

### WithdrawnAt

- type: **`<timestamp>`**
- Nullable: **`true`**
- default: **`null`**

### ScreenedAt

- type: **`<timestamp>`**
- Nullable: **`false`**
