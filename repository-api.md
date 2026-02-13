---
title: Repository API
category: Container
---

# {{ $frontmatter.title }}

[[toc]]

## Introduction

The Repository API is composed of two sets of data: Metadata and DataPDF: 

Metadata contains the structured data fields corresponding to an HPD record in the HPD Public Repository such as the Repository ID, HPD URL, Expiry Date, among others. These fields are searchable and allow API users to create queries to find HPDs that meet their specific criteria.

DataPDF contains data corresponding to all fields within the Health Product Declaration. 

Metadata structure can be found below. DataPDF structure can be found on the following section.

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
##Definitions

### CSIDivision

- type: **`<string>`**
- required: **`true`**
- Definition: The CSI Division corresponds to the CSI Masterformat Division number selected by the manufacturer.  

### CSISection

- type: **`<string>`**
- required: **`true`**
- Definition: The CSI Section corresponds to the CSI Masterformat Section number selected by the manufacturer.  

### CertificationsAndCompliance

- type: **`<string>`**
- required: **`false`**
- Definition: Summary list of compliance documentation reported by the manufacturer on Section 3: Compliance. 

### Characterized

- type: **`<string>`**
- required: **`false`**
- Definition: Indication of whether the manufacturer has reported weight and roles for all items in the content inventory. 

### Checksum

- type: **`<string>`**
- required: **`true`**
- Definition: The checksum is a unique identifier for the HPD. It can be used to determine if the HPD has been modified since it was created. 

### ContentInDescendingOrderOfQuantity

- type: **`<object>`**
- required: **`false`**
- default: **`null`**
- Definition: Summary list of content inventory items reported by the manufacturer in Section 2: Content Inventory.

### CreatedDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`**
- Definition: The date the HPD was first published.

### ExpiryDate

- type: **`<date>`**
- required: **`false`**
- default: **`null`** 
- Definition: The date the HPD expires.

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