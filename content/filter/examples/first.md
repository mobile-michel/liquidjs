---
title: first
description: Returns the first item of an array.
---

Input:  
{% raw %}
{{ product.first.title }}{% endraw %}

Output:
{{ product.first.title }}

Input:  
{% raw %}
{{ "Ground control to Major Tom." | split: " " | first }}{% endraw %}

Output:
{{ "Ground control to Major Tom." | split: " " | first }}