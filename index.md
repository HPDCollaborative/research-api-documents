---
title: What Is It?
lastUpdated: true
---

# {{ $frontmatter.title }}

[[toc]]

## Overview

This documentation is here to provide a reference for both incoming and outgoing data streams of the HPD Research API for [HPD Collaborative Open Standard v2.2.](https://www.hpd-collaborative.org/hpd-2-2-standard)

While outgoing data structures are not required to match the patterns described herein, it's recommended to follow these standard for consistency.

All incoming property values are set to Pascal Case and must be sent/received using exact Pascal Cased names shown here.

::: tip
Use the `Versions` dropdown menu top right of the page to view other versions of the documentation.
:::

## What to Expect

On each doc page you'll find a Structure section which will illustrate the shape of the data with type values, and then all properties available for the given data structure.

Let's make up a data object example widget.

## Structure

```json
{
  "Name": "<string>",
  "Quantity": "<int>",
  "Amount": "<float>",
  "Status": "<bool>",
  "Options": "<array|null>"
}
```

### Name

- type: **`<string>`**
- required: **`true`**

::: info
Occasionally you'll see additional notes if something needs to be noted or explained. Otherwise this box will not appear at all.
:::

### Quantity

- type: **`<int>`**
- required: **`true`**

::: danger IMPORTANT
Make sure you pay attention to `yellow` warning and `red` danger boxes for items that need special attention.
:::

### Amount

- type: **`<float>`**
- required: **`true`**

::: warning  
Numerical props will come in either `<int>` or `<float>`, make sure you note this in your internal storage.
:::

### Status

- type: **`<bool>`**
- required: **`true`**

::: info
Also watch for special `Dev Notes` which will provide additional code and are displayed in an accordion style panel with a right arrow as below:
:::

::: details Dev Note

- Important coder life hack below:

```php{6-8}
$fun = (new Jamesons())->drink(function($bottle) {
	try {
		return Life::today->finish($bottle)
			->without('spilling');
	} catch (E $spillage) {
		return TikTok::post($spillage->video)
			->then(Life::passout())
			->then(Life::tryAgainTomorrow());
	}
});
```

Just kidding ... don't drink and code! But you get the idea.

Most often what you'll see in this `Dev Note` is a diff reference from the previous version of the api.
:::

### Options

- type: **`<array>`**
- related: [Options](#)
- required: **`false`**
- default: **`<null|string>`**

::: tip  
Only props that are **NOT** required will have a default value, if at all. Props that show a `related` option are linked to their related data object.
:::

If you have any questions or issues, this repository is public so you can feel free to open a discussion at Github.
