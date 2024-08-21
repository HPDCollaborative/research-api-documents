---
title: Reference
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "Address1": "<string>",
  "Address2": "<string>",
  "City": "<string>",
  "State": "<string>",
  "Postal": "<string>",
  "Country": "<string>",
  "Website": "<string>",
  "Contact": "<string>",
  "Title": "<string>",
  "Phone": "<string>",
  "Email": "<string>",
  "Latitude": "<decimal:10,7>",
  "Longitude": "<decimal:10,7>",
  "PreparedBy": "<string>",
  "VerifiedBy": "<string>"
}
```

#### DIFF 2.2 > 2.3

```diff
+  "Latitude": "<decimal:10,7>",
+  "Longitude": "<decimal:10,7>",
```

### Address1

- type: **`<string>`**
- required: **`true`**

### Address2

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### City

- type: **`<string>`**
- required: **`true`**

### State

- type: **`<string>`**
- required: **`true`**

### Postal

- type: **`<string>`**
- required: **`true`**

### Country

- type: **`<string>`**
- required: **`true`**

### Website

- type: **`<string>`**
- required: **`true`**

### Contact

- type: **`<string>`**
- required: **`true`**

### Title

- type: **`<string>`**
- required: **`true`**

### Phone

- type: **`<string>`**
- required: **`true`**

### Email

- type: **`<string>`**
- required: **`true`**

### Latitude

- type: **`<decimal:10,7>`**
- required: **`false`**
- default: **`null|string`**

### Longitude

- type: **`<decimal:10,7>`**
- required: **`false`**
- default: **`null|string`**

### PreparedBy

- type: **`<int>`**
- required: **`false`**
- default: **`null|string`**

### VerifiedBy

- type: **`<int>`**
- required: **`false`**
- default: **`null|string`**
