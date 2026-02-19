---
title: Programs
category: Data
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
- Nullable: **`false`**

### Id

- type: **`<int>`**
- Nullable: **`false`**

### Name

- type: **`<string>`**
- Nullable: **`false`**

### Organization
- type: **`<string>`**
- Nullable: **`false`**

### Score
- type: **`<string>`**
- Nullable: **`false`**


### Updated
- type: **`<date>`**
- Nullable: **`false`**

### Version
- type: **`<date>`**
- Nullable: **`false`**