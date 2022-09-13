---
title: Introduction
lastUpdated: true
---

# {{ $frontmatter.title }}

[[toc]]

## Overview

The Content section represents the heart of an HPD. This is where you'll find:

- [Nested Materials](./nested-materials/)
- [Substances](./nested-materials/substances/)
- [Materials](./nested-materials/materials/)
- [Hazards](./nested-materials/substances/hazards.md)
- [Additional Listings](./nested-materials/substances/listings.md)
- [Special Conditions](./nested-materials/materials/special-conditions/biological.md)

## Inventory Reporting Format

HPDs can be created with two different inventory reporting formats:

- Nested Materials Method
- Basic Method

It's important to note that internally the same data structure is used for both. So in all cases, a Nested Materials array will be returned as the top level element in Content.

::: danger IMPORTANT
Just to reiterate and be clear, both Nested and Basic inventories will return an array of Nested Materials as the top level element in Content. Basic (method) will always return a single Nested Material, where Nested (method) can return many.
:::
