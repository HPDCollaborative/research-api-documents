---
title: Minor Fasteners Material
lastUpdated: true
outline: 'deep'
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> `{{ $frontmatter.title }}` is an addition to the 2.3 Standard.

## Structure

`{{ $frontmatter.title }}` is an object that can be attached to a [Material](../materials/) object under the `Condition` key.

```json
{
  "MinorFastener": {
    "ComponentComposition": "<string>",
    "EuRohsConformance": "<string>",
    "EuReachSvhcContent": "<string>",
    "EuRohsExemptions": "<string>",
    "SvhcDeclaration": "<string>",
    "LbcRedListCompliance": "<string>",
    "SpecialConditionThresholdDeclaration": "<string>"
  }
}
### ComponentComposition

- type: **`<string>`**
- required: **`true`**

### EuRohsConformance

- type: **`<string>`**
- required: **`true`**

### EuReachSvhcContent

- type: **`<string>`**
- required: **`true`**

### EuRohsExemptions

- type: **`<string>`**
- required: **`true`**

### SvhcDeclaration

- type: **`<string>`**
- required: **`true`**

### LbcRedListCompliance

- type: **`<string>`**
- required: **`true`**

### SpecialConditionThresholdDeclaration

- type: **`<string>`**
- required: **`true`**