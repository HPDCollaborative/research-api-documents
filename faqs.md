---
title: Frequently Asked Questions
category: Introduction
---

# {{ $frontmatter.title }}

[[toc]]

## General

### What is the purpose of this API?
The Research API allows you to access HPD data programmatically.

### How do I get an API token?
Please contact support to request an API token.

## Data

### How is the data structured?
The data is structured as a collection of JSON objects being the [Repository API](./repository-api) the start of the data object.


## Troubleshooting

### Why am I getting a 401 Unauthorized error?
Ensure you are including the `Token` parameter in your request query string.

### Why is the data field empty?
If the `Success` field is true but `Data` is empty, it means no records matched your query.

## HPD Structure Map

Below is a hierarchical map of the HPD structure starting from the Repository API.

```
[Repository API](./repository-api)
└──VocContent
└── DataPDFv3
    ├── General
    ├── Product
    ├── Parts
    ├── Certifications
    ├── Accessories
    ├── Notes
    ├── PFASData
    │   └── AttestationSignature
    ├── Programs
    └── Content 
        ├── NestedMaterials
            ├── Inventory
            ├── Substances
            │   ├── Hazards
            │   └── Listings
            └── Materials
                ├── Biological
                ├── Geological
                ├── Mixed Content
                ├── Electronics
                ├── Fasteners
                ├── Metal Alloys
                │   └── GreenScreenAlloyingElements
                └── Polymers
                │   ├── With CASRN
                │   ├── Without CASRN
                │   └── Undisclosed
```
