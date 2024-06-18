---
title: sort_natural
description: Sorts items in an array in case-insensitive order.
---
Input:  
{% raw %}{% assign my_array = "zebra, octopus, giraffe, Sally Snake" | split: ", " %}  
{{ my_array | sort_natural | join: ", " }}{% endraw %}

Output: 
{% assign my_array = "zebra, octopus, giraffe, Sally Snake" | split: ", " %}
{{ my_array | sort_natural | join: ", " }}

An optional argument specifies which property of the array’s items to use for sorting:

Input:  
{% raw %}{% assign products_by_category = pages.products | sort_natural: "category" %}  
{% for product in products_by_category %}  
{{ product.category }}  
{%- endfor %}{% endraw %}

Output:  
{% assign products_by_category = pages.products | sort_natural: "category" %}
{% for product in products_by_category %}
- {{ product.category }}
{%- endfor %}