---
title: join
description: Combines the items in an array into a single string using the argument as a separator.
---
{% for item in product %}
- {{ item.title }}
{% endfor %}

Input:  
{% raw %}
{% assign items = product.title %}
{{ items | join: " and " }}{% endraw %}

Output:
{% assign items = product.title %}
{{ items | join: " and " }}

Input:  
{% raw %}
{% assign beatles = "John, Paul, George, Ringo" | split: ", " %}
{{ beatles | join: " and " }}{% endraw %}

Output:
{% assign beatles = "John, Paul, George, Ringo" | split: ", " %}
{{ beatles | join: " and " }}