---
title: Repository API
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Introduction

The Repository API is composed of two sets of data: Metadata and DataPDF: 
Metadata contains the structured data fields corresponding to an HPD record in the HPD Public Repository such as the Repository ID, HPD URL and HPD versions

DataPDF contains data corresponding to all fields within the Health Product Declaration. Data PDF is reported in two buckets: HPD Data Other Sections and HPD Data Content Inventory

Repository API
  -DataPDF 
    -Content
      -Conditions
      -Substances
      -Polymers


## Structure

```json
[
  {
    "CSIDivision": "<string>",
    "CSISection": "<string>",
    "CertificationsAndCompliance": "<string>",
    "Characterized": "<string>",
    "Checksum": "<string>",
    "ContentInDescendingOrderOfQuantity": "<object>",
    "CreatedDate": "<date>",
    "DataPDFv3": "<object>",
    "ExpiryDate": "<date>",
    "HPDUrl": "<string>",
    "HPDVersion": "<string>",
    "ID": "<string>",
    "Identified": "<string>",
    "InventoryType": "<string>",
    "LEEDv4": "<string>",
    "ManufacturerAddress": "<string>",
    "ManufacturerContactName": "<string>",
    "ManufacturerContactPhoneNumber": "<string>",
    "ManufacturerContactTitle": "<string>",
    "ManufacturerEmail": "<string>",
    "ManufacturerName": "<string>",
    "ManufacturerWebsite": "<string>",
    "ModifiedDate": "<date>",
    "Nanomaterial": "<string>",
    "NumberOfGreenScreenBMContents": "<string>",
    "Preparer": "<string>",
    "ProductDescription": "<string>",
    "ProductName": "<string>",
    "PublishedDate": "<date>",
    "ResidualsImpurities": "<string>",
    "Screened": "<string>",
    "ScreeningDate": "<date>",
    "ThirdPartyVerified": "<string>",
    "ThresholdDisclosedPer": "<string>",
    "ThresholdLevel": "<string>",
    "Title": "<string>",
    "UniqueId": "<string>",
    "VOCContent": "<object>",
    "Verifier": "<string>",
    "Version": "<string>",
    "Versions":"<array>"
  }
]
```

### CSIDivision

- type: **`<string>`**
- required: **`true`**

### CSISection

- type: **`<string>`**
- required: **`true`**

### CertificationsAndCompliance

- type: **`<string>`**
- required: **`false`**

### Characterized

- type: **`<string>`**
- required: **`false`**

### Checksum

- type: **`<string>`**
- required: **`true`**

### ContentInDescendingOrderOfQuantity

- type: **`<object>`**
- required: **`false`**
- default: **`null`**

### CreatedDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`**

### ExpiryDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`**

### HPDUrl

- type: **`<string>`**
- required: **`false`**

### HPDVersion

- type: **`<string>`**
- required: **`false`**

### ID

- type: **`<string>`**
- required: **`false`**

### Identified

- type: **`<string>`**
- required: **`false`**

### InventoryType

- type: **`<string>`**
- required: **`false`**

### LEEDv4

- type: **`<string>`**
- required: **`false`**

### ManufacturerAddress

- type: **`<string>`**
- required: **`false`**

### ManufacturerContactName

- type: **`<string>`**
- required: **`false`**

### ManufacturerContactPhoneNumber

- type: **`<string>`**
- required: **`false`**

### ManufacturerContactTitle

- type: **`<string>`**
- required: **`false`**

### ManufacturerEmail

- type: **`<string>`**
- required: **`false`**

### ManufacturerName

- type: **`<string>`**
- required: **`false`**

### ManufacturerWebsite

- type: **`<string>`**
- required: **`false`**

### ModifiedDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`**

### Nanomaterial

- type: **`<string>`**
- required: **`false`**

### NumberOfGreenScreenBMContents

- type: **`<string>`**
- required: **`false`**


### Preparer

- type: **`<string>`**
- required: **`false`**

### ProductDescription

- type: **`<string>`**
- required: **`false`**

### ProductName

- type: **`<string>`**
- required: **`false`**

### PublishedDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`**

### ResidualsImpurities

- type: **`<string>`**
- required: **`false`**

### Screened

- type: **`<string>`**
- required: **`false`**

### ScreeningDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`**

### ThirdPartyVerified

- type: **`<string>`**
- required: **`false`**

### ThresholdDisclosedPer

- type: **`<string>`**
- required: **`false`**

### ThresholdLevel

- type: **`<string>`**
- required: **`false`**

### Title

- type: **`<string>`**
- required: **`true`**

### UniqueId

- type: **`<string>`**
- required: **`true`**

### VOCContent

- type: **`<object>`**
- required: **`false`**
- default: **`null`**

### Verifier

- type: **`<string>`**
- required: **`true`**

### Version

- type: **`<string>`**
- required: **`true`**
- default: **1.0**

### Versions

- type: **`<array>`**
- required: **`false`**
- default: **`[]`**