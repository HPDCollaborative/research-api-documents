---
title: Certifications and Compliance
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
[
  {
    "Type": "<string>",
    "OtherType": "<string>",
    "Name": "<string>",
    "Voc": "<string>",
    "Party": "<string>",
    "Issue": "<date>",
    "Expire": "<date>",
    "Lab": "<string>",
    "Facilities": "<string>",
    "Website": "<string>",
    "Notes": "<string>",
    "ComplianceDetails": "<string>",
    "ComplianceScope": "<string>"
  }
]
```
#### DIFF 2.32 > 3.0
```diff
+   "ComplianceDetails": "<string>"
+   "ComplianceScope": "<string>"
```
### Type

- type: **`<string>`**
- Nullable: **`false`**

### OtherType

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null`**

### Name

- type: **`<string>`**
- Nullable: **`false`**

### Voc

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null`**

### Party

- type: **`<string>`**
- Nullable: **`false`**

### Issue

- type: **`<date>`**
- Nullable: **`true`**
- default: **`null`**

### Expire

- type: **`<date>`**
- Nullable: **`true`**
- default: **`null`**

### Lab

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null`**

### Facilities

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null`**

### Website

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null`**

### Notes

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null`**
