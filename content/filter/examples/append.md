---
title: append
description: Concatenates two strings and returns the concatenated value.
---
**{% raw %}{{ "/my/fancy/url" | append: ".html" }}{% endraw %}**: {{ "/my/fancy/url" | append: ".html" }}

`Append` can also be used with variables:

**{% raw %}{% assign filename = "/index.html" %}
{{ "website.com" | append: filename }}{% endraw %}**: {% assign filename = "/index.html" %}
{{ "website.com" | append: filename }}