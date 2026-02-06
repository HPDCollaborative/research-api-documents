---
title: Product
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> Precheck Programs that the HPD was checked against on the Builder

## Structure

```json
{
    "Created": "<date>",
    "Criteria": "<object>",
    "Hash": "<string>",
    "Id": "<int>",
    "Name": "<string>",
    "Organization": "<string>",
    "ProgramLogoUrl": "<string>",
    "Results": "<object>",
    "Score": "<string>",
    "Slug": "<string>",
    "Updated": "<date>",
    "Version": "<date>"
}
```

### Created

- type: **`<date>`**
- required: **`true`**

### Criteria

- type: **`<object>`**
- required: **`true`**

### Hash

- type: **`<string>`**
- required: **`true`**

#### Id

- type: **`<int>`**
- required: **`true`**

### Name

- type: **`<string>`**
- required: **`true`**

### Organization
- type: **`<string>`**
- required: **`true`**

### ProgramLogoUrl
- type: **`<string>`**
- required: **`true`**

### Results
- type: **`<string>`**
- required: **`true`**

### Score
- type: **`<string>`**
- required: **`true`**

### Slug
- type: **`<string>`**
- required: **`true`**

### Updated
- type: **`<date>`**
- required: **`true`**

### Version
- type: **`<date>`**
- required: **`true`**