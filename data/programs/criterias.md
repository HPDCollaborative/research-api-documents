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
- Nullable: **`true`**
#### InventoryType
- type: **`<string>`**
- Nullable: **`true`**
#### MinimumThresholdAllowed
- type: **`<string>`**
- Nullable: **`true`**
#### Screened
- type: **`<string>`**
- Nullable: **`true`**
#### ThirdPartyVerified
- type: **`<string>`**
- Nullable: **`true`**
#### ThresholdDisclosure
- type: **`<string>`**
- Nullable: **`true`**


### Required

#### Characterized
- type: **`<string>`**
- Nullable: **`true`**
#### InventoryType
- type: **`<string>`**
- Nullable: **`true`**
#### MinimumThresholdAllowed
- type: **`<string>`**
- Nullable: **`true`**
#### Screened
- type: **`<string>`**
- Nullable: **`true`**
#### ThirdPartyVerified
- type: **`<string>`**
- Nullable: **`true`**
#### ThresholdDisclosure
- type: **`<string>`**
- Nullable: **`true`**

### Screening

#### Concerns
- type: **`<array>`**
- Nullable: **`true`**


#### Redlists
- type: **`<array>`**
- Nullable: **`true`**
