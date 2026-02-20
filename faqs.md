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

- [Repository API](./repository-api)
  - [DataPDFv3](./data/)
    - [General](./data/general)
    - [Product](./data/product)
    - [Parts](./data/parts)
    - [Certifications](./data/certifications)
    - [Accessories](./data/accessories)
    - [Notes](./data/notes)
    - [PFASData](./data/pfasdata)
      - [AttestationSignature](./data/pfasdata/AttestationSignature)
    - [Programs](./data/programs)
    - [Content](./content/)
      - [NestedMaterials](./content/nested-materials/)
        - [Locations](./content/locations)
        - [Substances](./content/substances/)
          - [Hazards](./content/substances/hazards)
          - [Listings](./content/substances/listings)
        - [Materials](./content/materials/)
          - [Biological](./content/materials/biological)
          - [Geological](./content/materials/geological)
          - [Mixed Content](./content/materials/mixed-content)
          - [Electronics](./content/materials/electronics)
          - [Fasteners](./content/materials/fasteners)
          - [Metal Alloys](./content/materials/metal-alloys)
            - [GreenScreenAlloyingElements](./content/materials/metal-alloys/GreenScreenAlloyingElements)
          - [Polymers](./content/polymers/)
            - [With CASRN](./content/polymers/with-casrn)
            - [Without CASRN](./content/polymers/without-casrn)
            - [Undisclosed](./content/polymers/undisclosed)
