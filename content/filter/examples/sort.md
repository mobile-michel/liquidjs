---
title: sort
description: Sorts items in an array in case-sensitive order.
---
Input:  
{% raw %}{% assign my_array = "zebra, octopus, giraffe, Sally Snake" | split: ", " %}  
{{ my_array | sort | join: ", " }}{% endraw %}

Output: 
{% assign my_array = "zebra, octopus, giraffe, Sally Snake" | split: ", " %}
{{ my_array | sort | join: ", " }}

An optional argument specifies which property of the array’s items to use for sorting:

Input:  
{% raw %}{% assign products_by_category = pages.products | sort: "category" %}  
{% for product in products_by_category %}  
{{ product.category }}  
{%- endfor %}{% endraw %}

Output:  
{% assign products_by_category = pages.products | sort: "category" %}
{% for product in products_by_category %}
- {{ product.category }}
{%- endfor %}