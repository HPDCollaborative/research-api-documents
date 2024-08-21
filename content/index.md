---
title: Introduction
category: Content
---

# {{ $frontmatter.title }}

[[toc]]

## Overview

The Content section represents the heart of an HPD. This is where you'll find:

- [Nested Materials](./nested-materials/)
- [Substances](./substances/)
- [Materials](./materials/) _(formerly Special Conditions)_
- [Hazards](./substances/hazards)
- [Additional Listings](./substances/listings)
- [Polymers](./polymers)
- [Locations](./locations)

## Inventory Reporting Format

HPDs can be created with two different inventory reporting formats:

- Nested Materials Method
- Basic Method

It's important to note that internally the same data structure is used for both. So in all cases, a Nested Materials array will be returned as the top level element in Content.

::: danger IMPORTANT
Just to reiterate and be clear, both Nested and Basic inventories will return an array of Nested Materials as the top level element in Content. Basic (method) will always return a single Nested Material, where Nested (method) can return many.
:::
