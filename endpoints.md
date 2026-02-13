---
title: Endpoints
category: Introduction
---

# {{ $frontmatter.title }}

[[toc]]

## Postman
You can find the Postman documentation in the following link:
https://documenter.getpostman.com/view/2852259/TVspjUMV

---
## Endpoints Structure
```json
{
  "Data": <Array/Object>,
  "Message": <String>,
  "Success": <Boolean>
}
```

## Get All HPDs
This endpoint allows you to get all the HPDs.

GET **GetAllHPDsv3?Page={#Pages}&Rows=10&Token={{Token}}**


### Query Parameters

| Parameter | Type | Description |
|-----------|--------|-------------|
| Rows | integer | Number of HPDs returned per request (page size). |
| Page | integer | Page number to retrieve (1-based index). For example, `Page=1` returns the first set of results, `Page=2` returns the next set. |
| Token | string | Authentication token provided to your company. |
---
### Response Fields

| Field | Type | Description |
|--------|--------|-------------|
| Data | array | Array of HPD objects. |
| Message | string | Pagination summary describing the returned range (e.g., `"HPDs 11 to 20 of 145"`). |
| Success | boolean | Indicates wh  ether the request was successful (`true` or `false`). |

## Get HPD by ID
This endpoint allows you to get a single HPD by ID

GET **/GetHPDv3?Token={{Token}}&ID={{ID}}**

### Query Parameters

| Parameter | Type | Description |
|-----------|--------|-------------|
| ID | integer | ID of the HPD according to the ID field on the repository  |
| Token | string | Authentication token provided to your company. |
---
### Response Fields

| Field | Type | Description |
|--------|--------|-------------|
| Data | object | Single HPD |
| Message | string | Text message showing if the HPD was found (e.g., `"HPD with ID:41960, found"`). |
| Success | boolean | Indicates whether the request was successful (`true` or `false`). |

## Get HPD by Filename
This endpoint allows you to get a single HPD by Filename
GET **/GetHPDFileNamev3?Filename={{Filename}}f&Token={{Token}}**

### Query Parameters

| Parameter | Type | Description |
|-----------|--------|-------------|
| Filename | integer | ID of the HPD according to the ID field on the repository  |
| Token | string | Authentication token provided to your company. |
---
### Response Fields

| Field | Type | Description |
|--------|--------|-------------|
| Data | object | Single HPD |
| Message | string | Text message showing if the HPD was found (e.g., `"HPD  found"`). |
| Success | boolean | Indicates whether the request was successful (`true` or `false`). |

## Get HPD by Query
The HPD Get by Query method allows for more complex searches using CAML (Collaborative Application Markup Language) queries.

GET **GetAllHPDsv3?Page={#Pages}&Rows=10&Token={{Token}}**


### Query Parameters

| Parameter | Type | Description |
|-----------|--------|-------------|
| Query | String | Query that follows the schema of Collaborative Application Markup Language (CAML)  |
| Rows | integer | Number of HPDs returned per request (page size). |
| Page | integer | Page number to retrieve (1-based index). For example, `Page=1` returns the first set of results, `Page=2` returns the next set. |
| Token | string | Authentication token provided to your company. |
---
### Response Fields

| Field | Type | Description |
|--------|--------|-------------|
| Data | array | Array of HPD objects. |
| Message | string | Pagination summary describing the returned range (e.g., `"HPDs 11 to 20 of 145"`). |
| Success | boolean | Indicates whether the request was successful (`true` or `false`). |

### CAML Query
 Below is the mapping of common field names to their internal SharePoint names required for these queries.
For more information on how CAML Query works you can check on https://learn.microsoft.com/en-us/sharepoint/dev/schema/query-schema. 

#### Example of queries
Below are examples of how to structure the `query` parameter for the HPD Get by Query method.

#### 1. Query by unique_id
```xml
<Where>
  <Eq> 
    <FieldRef Name='unique_id_TXT' /> 
    <Value Type='Text'>26311</Value>
  </Eq>
</Where>
```
#### 2. Get All HPDs that contains a specific CSI Section
```xml
<Where>
    <Contains>
      <FieldRef Name='csi_section' />
      <Value Type='Text'>09 30 13</Value>
    </Contains>
</Where>
```
#### 3.Get All HPDS Created or Modified after date
```xml
<Where>
  <Or>
    <Geq>
      <FieldRef Name='Created' />
      <Value Type='DateTime'>2022-08-18T01:00:00.000Z</Value>
    </Geq>
    <Geq>
      <FieldRef Name='Modified' />
      <Value Type='DateTime'>2022-08-18T01:00:00.000Z</Value>
    </Geq>
  </Or>
</Where>
```
#### 4. Get the HPDs with that have csi section that begins with text
```xml
<Where>
  <BeginsWith>
    <FieldRef Name='csi_section' />
    <Value Type='Text'>09 6</Value>
  </BeginsWith>
</Where>
```
#### 5. Get all the HPDs that have already expired before today
```xml
<Where>
  <Lt>
    <FieldRef Name='Expiry_x0020_Date' />
    <Value Type='DateTime'><Today /></Value>
  </Lt>
</Where>
```
#### 6. Get all the HPDs that have not expired before today
```xml
<Where>
  <Geq>
    <FieldRef Name='Expiry_x0020_Date' />
    <Value Type='DateTime'><Today /></Value>
  </Geq>
</Where>
```
#### 7. Get all the HPDs that contain a keyword in the product name field
```xml
<Where>
  <Contains>
    <FieldRef Name='Product_x0020_Name' />
    <Value Type='Text'>REBAR</Value>
  </Contains>
</Where>
```
#### Internal Field names
Use the Internal Name of the fields to be able to use it on a query

| Field Name | Internal Name | Type |
| :--- | :--- | :--- |
| Name | FileLeafRef | File |
| Title | Title | Text |
| Product Name | Product_x0020_Name | Text |
| Manufacturer Name | Manufacturer_x0020_Name | Text |
| HPD Version | HPD_x0020_Version | Choice |
| CSI Division | csi_division | Text |
| CSI Section | csi_section | Text |
| LEED v4 | LEED_x0020_v4 | Choice |
| Expiry Date | Expiry_x0020_Date | DateTime |
| File Checksum | Checksum | Text |
| Inventory Type | Inventory_x0020_Type | Choice |
| Publication Status | Publication_x0020_Status | Choice |
| Screening Methodology | Screening_x0020_Methodology | Choice |
| LEED v4 Methodology | LEED_x0020_v4_x0020_Methodology | Choice |
| Manufacturer Email | Manufacturer_x0020_Email | Text |
| Third Party Verified | Third_x0020_Party_x0020_Verified | Boolean |
| Created | Created | DateTime |
| Modified | Modified | DateTime |
| unique_id | unique_id_TXT | Text |

## Get All Withdrawn HPDs
This endpoint allows you to get all the HPDs that have been withdrawn from the repository.

GET **/GetAllWithdrawnHPDs?Page=1&Rows=10&Token={{Token}}**


### Query Parameters

| Parameter | Type | Description |
|-----------|--------|-------------|
| Rows | integer | Number of HPDs returned per request (page size). |
| Page | integer | Page number to retrieve (1-based index). For example, `Page=1` returns the first set of results, `Page=2` returns the next set. |
| Token | string | Authentication token provided to your company. |
---
### Response Fields

| Field | Type | Description |
|--------|--------|-------------|
| Data | array | Array of Withdrawn HPD objects. |
| Message | string | Pagination summary describing the returned range (e.g., `"Withdrawn HPDs from 11 to 20 of 145"`). |
| Success | boolean | Indicates whether the request was successful (`true` or `false`). |


### Withdrawn HPD

```json
{
  "Comments": <string>,
  "DeletedDate": <date>,
  "Filename": <string>,
  "HPDVersion": <string>,
  "ID": <int>,
  "Title": <string>,
  "UniqueId": <string>
}
```
Here is the Field Definitions table for the JSON response fields, formatted as requested within a markdown code block:

Markdown
| Field | Type | Description |
| :--- | :--- | :--- |
| **Comments** | string | Descriptive notes or additional context provided regarding the HPD deletion. |
| **DeletedDate** | date | The timestamp indicating when the document was removed or archived from the active repository. |
| **Filename** | string | The specific name of the stored file, typically used to download or reference the PDF. |
| **HPDVersion** | string | The version of the Health Product Declaration standard (e.g., 2.2, 2.3,3.0). |
| **ID** | int | The unique ID assigned by the repository to track the record internally. |
| **Title** | string | The display title of the HPD,  |
| **UniqueId** | string | A unique text-based identifier found in the HPD