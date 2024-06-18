---
title: prepend
description: Adds the specified string to the beginning of another string.
---
**{% raw %}{{ "apples, oranges, and bananas" | prepend: "Some fruit: " }}{% endraw %}**: {{ "apples, oranges, and bananas" | prepend: "Some fruit: " }}

`prepend` can also be used with variables:

**{% raw %}{% assign url = "example.com" %}
{{ "/index.html" | prepend: url }}{% endraw %}**: {% assign url = "example.com" %}
{{ "/index.html" | prepend: url }}