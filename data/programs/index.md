---
title: Product
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Structure

```json
{
    "Name": "<string>",
    "Organization": "<string>",
    "ProgramLogoUrl": "<string>",
    "Results": {
        "Listings": {
        "Fail": "<int>",
        "Pass": "<int>",
        "Total": "<int>",
        "Warn": "<int>"
        },
        "Preferred": {
        "Fail": "<int>",
        "Pass": "<int>",
        "Total": "<int>",
        "Warn": "<int>"
        },
        "Redlists": {
        "Fail": "<int>",
        "Pass": "<int>",
        "Total": "<int>",
        "Warn": "<int>"0
        },
        "Required": {
        "Fail": "<int>",
        "Pass": "<int>",
        "Total": "<int>",
        "Warn": "<int>"
        }
    },
    "Score": "<string>",
    "Slug": "<string>",
    "Updated": "<date>",
    "Version": "<date>"
}
```

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