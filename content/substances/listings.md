---
title: Listings
category: Content
---

# {{ $frontmatter.title }}

::: info
Listings is a new data array that represents Additional Hazard Listings.
:::

[[toc]]

## Structure

Listings, if included, exist as an array of Listing objects listed with the key of `Listings` and are structured as follows:

```json
[ // Start of "Listings" array
  {
    "Listing": "<string>",
    "Agency": "<string>",
    "Notification": "<string>"
  }
  ...
]
```

#### DIFF 2.2 > 2.3

```diff
+ "Listings": [
+   {
+     "Listing": "<string>",
+     "Agency": "<string>",
+     "Notification": "<string>"
+   }
+ ]
```

### Listing

- type: **`<string>`**
- required: **`true`**

### Agency

- type: **`<string>`**
- required: **`true`**

### Notification

- type: **`<string>`**
- required: **`true`**
