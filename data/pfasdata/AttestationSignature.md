---
title: Attestation Signature
category: PFAS Data
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
  "SignaturePath": "<string>",
  "SignatureText": "<string>",
  "Type": "image|text"
}
```

### SignaturePath

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

::: tip
The complete path to the signature image file is composed of the `BaseUrl` and the `SignaturePath`.
Example: `https://hpdrepository.hpd-collaborative.org/repository/` + `SignaturePath`
:::

### SignatureText

- type: **`<string>`**
- required: **`false`**
- default: **`null|string`**

### Type

- type: **`<string>`**
- required: **`false`** 
- Values: **`image`**, **`text`**
