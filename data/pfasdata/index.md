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
- Nullable: **`true`**
- default: **`null|string`**

### AttestationSignature

- type: **`<object>`**
- Nullable: **`true`**
- default: **`null|object`**
- related: [Attestation Signature](./AttestationSignature)

### PfasStatus

- type: **`<string>`**
- Nullable: **`true`**
- default: **`null|string`**

### AttestationDate

- type: **`<date>`**
- Nullable: **`true`**
- default: **`null|date`**
