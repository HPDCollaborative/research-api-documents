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
  "Message": <String>
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
| Message | string | Pagination summary describing the returned range (e.g., `"HPDs 11–20 of 145"`). |
| Success | boolean | Indicates whether the request was successful (`true` or `false`). |

