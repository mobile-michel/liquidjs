---
title: last
description: Returns the last item of an array.
---

Input:  
{% raw %}
{{ product.last.title }}{% endraw %}

Output:
{{ product.last.title }}

Input:  
{% raw %}
{{ "Ground control to Major Tom." | split: " " | last }}{% endraw %}

Output:
{{ "Ground control to Major Tom." | split: " " | last }}