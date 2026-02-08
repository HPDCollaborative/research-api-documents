---
title: PFAS Data
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "PfasMessage": "<string>",
  "AttestationSignature": {
    "Type": "<string>",
    "Signature": "<string>",
  },
  "PfasStatus": "<string>",
  "AttestationDate": "<date>"
}
```

### PfasMessage

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### AttestationSignature

- type: **`<object>`**
```json
"AttestationSignature": {
    "Type": "<string>",
    "Signature": "<string>",
  }
```
- required: **`false`**
- default: **`null|object`**

### PfasStatus

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### AttestationDate

- type: **`<date>`**
- required: **`false`**
- default: **`null|date`**
