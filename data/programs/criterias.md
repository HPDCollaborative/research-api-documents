---
title: Criteria
category: Programs
---

# {{ $frontmatter.title }}

[[toc]]

> [!INFO]
> Criteria based on the program prechecks

## Structure

```json
"Criteria": {
    "Preferred": {
        "Characterized": "<string>",
        "InventoryType": "<string>",
        "MinimumThresholdAllowed": "<string>",
        "Screened": "<string>",
        "ThirdPartyVerified": "<string>",
        "ThresholdDisclosure": "<string>"
    },
    "Required": {
        "Characterized": "<string>",
        "InventoryType": "<string>",
        "MinimumThresholdAllowed": "<string>",
        "Screened": "<string>",
        "ThirdPartyVerified": "<string>",
        "ThresholdDisclosure": "<string>"
    },
    "Screening": {
        "Concerns": ["<string>"],
        "Redlists": ["<string>"]
    }
}
```

### Preferred

#### Characterized
- type: **`<string>`**
- required: **`false`**
#### InventoryType
- type: **`<string>`**
- required: **`false`**
#### MinimumThresholdAllowed
- type: **`<string>`**
- required: **`false`**
#### Screened
- type: **`<string>`**
- required: **`false`**
#### ThirdPartyVerified
- type: **`<string>`**
- required: **`false`**
#### ThresholdDisclosure
- type: **`<string>`**
- required: **`false`**


### Required

#### Characterized
- type: **`<string>`**
- required: **`false`**
#### InventoryType
- type: **`<string>`**
- required: **`false`**
#### MinimumThresholdAllowed
- type: **`<string>`**
- required: **`false`**
#### Screened
- type: **`<string>`**
- required: **`false`**
#### ThirdPartyVerified
- type: **`<string>`**
- required: **`false`**
#### ThresholdDisclosure
- type: **`<string>`**
- required: **`false`**

### Screening

#### Concerns
- type: **`<array>`**
- required: **`false`**


#### Redlists
- type: **`<array>`**
- required: **`false`**
