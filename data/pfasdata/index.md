---
title: PFAS Data
category: Data
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
- required: **`false`**
- default: **`null|object`**
- related: [Attestation Signature](../AttestationSignature/)

### PfasStatus

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### AttestationDate

- type: **`<date>`**
- required: **`false`**
- default: **`null|date`**
