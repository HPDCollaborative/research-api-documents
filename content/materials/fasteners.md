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
- Nullable: **`false`**

### EuRohsConformance

- type: **`<string>`**
- Nullable: **`false`**

### EuReachSvhcContent

- type: **`<string>`**
- Nullable: **`false`**

### EuRohsExemptions

- type: **`<string>`**
- Nullable: **`false`**

### SvhcDeclaration

- type: **`<string>`**
- Nullable: **`false`**

### LbcRedListCompliance

- type: **`<string>`**
- Nullable: **`false`**

### SpecialConditionThresholdDeclaration

- type: **`<string>`**
- Nullable: **`false`**