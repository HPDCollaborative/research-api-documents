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
