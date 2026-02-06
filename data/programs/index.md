---
title: Product
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> Precheck Programs that the HPD was checked against on the Builder. Is shown as aligned or not aligned if the program didn't pass

## Structure

```json
{
    "Created": "<date>",
    "Id": "<int>",
    "Name": "<string>",
    "Organization": "<string>",
    "Score": "<string>",
    "Updated": "<date>",
    "Version": "<date>"
}
```

### Created

- type: **`<date>`**
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

### Score
- type: **`<string>`**
- required: **`true`**


### Updated
- type: **`<date>`**
- required: **`true`**

### Version
- type: **`<date>`**
- required: **`true`**