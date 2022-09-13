---
title: Accessories
lastUpdated: true
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
[
  {
    "Name": "<string>",
    "Website": "<string>",
    "AccessoryType": "<string>",
    "Manufacturer": "<string>",
    "Notes": "<string>"
  }
]
```

#### DIFF 2.2 > 2.3

```diff
-   "Conditions": "<string>"
+   "AccessoryType": "<string>"
+   "Manufacturer": "<string>"
+   "Notes": "<string>"
```

---

### Name

- type: **`<string>`**
- required: **`true`**

### Website

- type: **`<string>`**
- required: **`true`**

### AccessoryType

- type: **`<string>`**
- required: **`true`**

### Manufacturer

- type: **`<string>`**
- required: **`true`**

### Notes

- type: **`<string>`**
- required: **`false`**
- default: **`string`**
