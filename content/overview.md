---
title: Introduction
category: Content
---

# {{ $frontmatter.title }} {.doc-heading}

[[toc]]

## Overview {.doc-heading}

The Content section represents the heart of an HPD. This is where you'll find:

- [Materials](./materials/)
- [Substances](./materials/substances/)
- [Hazards](./materials/substances/hazards.md)

## Inventory Reporting Format {.doc-heading}

HPDs can be created with two different inventory reporting formats:

- Nested Materials Method
- Basic Method

It's important to note that internally the same data structure is used for both. So in all cases, a Materials array will be returned as the top level element in Content.

::: danger IMPORTANT
Just to reiterate and be clear, both Nested and Basic inventories will return an array of Materials as the top level element in Content. Basic will always return a single Material, where Nested can return many.
:::
