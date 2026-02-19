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
    "ID": "<int>",
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
## Definitions
### CSIDivision

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The CSI Division corresponds to the CSI Masterformat Division number selected by the manufacturer.`**  

### CSISection

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The CSI Section corresponds to the CSI Masterformat Section number selected by the manufacturer.`**  

### CertificationsAndCompliance

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Summary list of compliance documentation reported by the manufacturer on Section 3: Compliance.`**

### Characterized

- type: **`<string>`**
- Nullable: **`true`**
- Values: **`Yes`**, **`Yes Ex/SC`**, **`No`**
- Definition: **`Indication of whether the manufacturer has reported weight and roles for all items in the content inventory.`** 

### Checksum

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The checksum is a unique identifier for the HPD. It can be used to determine if the HPD has been modified since it was created.`** 

### ContentInDescendingOrderOfQuantity

- type: **`<object>`**
- Nullable: **`true`**
- Definition: **`Summary list of content inventory items reported by the manufacturer in Section 2: Content Inventory.`**

### CreatedDate

- type: **`<date>`**
- Nullable: **`true`**
- Definition: **`The date the HPD was first published.`**

### ExpiryDate

- type: **`<date>`**
- Nullable: **`true`**
- Definition: **`The date the HPD expires. Normally 3 years from the published date.`**

### DataPDFv3

- type: **`<object>`**
- Nullable: **`true`**
- related: [DataPDF](./data)
- Definition: **`The DataPDFv3 is the HPD data in a structured format.`**

### HPDUrl

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The URL link to the HPD data file.`**

### HPDVersion

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The version of the HPD Open Standard.`**

### ID

- type: **`<int>`**
- Nullable: **`true`**
- Definition: **`The unique identifier for the HPD on the repository, this ID is used to retrieve a single HPD record with the Get HPD by ID endpoint.`**

### Identified

- type: **`<string>`**
- Nullable: **`true`**
- Values: **`Yes`**, **`Yes Ex/SC`**, **`No`**
- Definition: **` An HPD is marked as "Identified" when the name (specific or generic) and identifier are provided for every ingredient, supporting transparency in material health and building products.`**

### InventoryType

- type: **`<string>`**
- Nullable: **`false`**
- Values: **`nested`**, **`basic`**
- Definition: **`The type of how the contents are reported, nested or basic`**

### LEEDv4

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The LEEDv4 prechecks the HPD has`**

### ManufacturerAddress

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The address of the manufacturer.`**

### ManufacturerContactName

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The name of the contact person for the manufacturer.`**

### ManufacturerContactPhoneNumber

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The phone number of the contact person for the manufacturer.`**

### ManufacturerContactTitle

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The title of the contact person for the manufacturer.`**

### ManufacturerEmail

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The email address of the contact person for the manufacturer.`**

### ManufacturerName

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The name of the manufacturer.`**

### ManufacturerWebsite

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The website of the manufacturer.`**

### ModifiedDate

- type: **`<date>`**
- Nullable: **`true`**
- default: **`null`**
- Definition: **`The date the HPD was last modified.`**

### Nanomaterial

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Indication of whether the manufacturer has reported nanomaterials in the content inventory.`**

### NumberOfGreenScreenBMContents

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The number of Green Screen Benchmark contents in the content inventory.`**


### Preparer

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`If prepared by the manufacturer, "Self-Prepared" is inserted; if prepared by a third party, the name of the organization is inserted.`**

### ProductDescription

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Brief description of the product`**

### ProductName

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Product brand name`**

### PublishedDate

- type: **`<date>`**
- Nullable: **`true`**
- Definition: **`The date the HPD was published.`**

### ResidualsImpurities

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Indication of whether the manufacturer has reported residuals and impurities in the content inventory.`**

### Screened

- type: **`<string>`**
- Nullable: **`true`**
- Values: **`Yes`**, **`Yes Ex/SC`**, **`No`**
- Definition: **`Indication of whether the manufacturer has reported screened contents in the content inventory.`**

### ScreeningDate

- type: **`<date>`**
- Nullable: **`true`**
- Definition: **`The date the HPD was screened.`**

### ThirdPartyVerified

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Indication of whether the HPD has been third-party verified.`**

### ThresholdDisclosedPer

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`Indicates if the screening for hazards (e.g., in a product like a hand dryer or furniture) was conducted at the material or product level.`**

### ThresholdLevel

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The threshold level at which the manufacturer has disclosed the contents of the HPD.`**

### Title

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`Title of the HPD used on the repository composed by Product Name / Manufacturer Name / Expiry Date.`**

### UniqueId

- type: **`<string>`**
- Nullable: **`false`**
- Definition: **`The unique identifier for the HPD on the repository.`**

### VOCContent

- type: **`<object>`**
- Nullable: **`true`**
- related: [VOC](/data/voc)
- Definition: **`The VOC content of the HPD.`**

### Verifier

- type: **`<string>`**
- Nullable: **`true`**
- Definition: **`The verifier of the HPD.`**

### Version

- type: **`<string>`**
- Nullable: **`false`**
- default: **1.0**
- Definition: **`The version of the HPD, how many times the HPD has been published.`**