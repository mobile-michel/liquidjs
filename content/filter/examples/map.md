---
title: map
description: Creates an array of values by extracting the values of a named property from another object.
---
Input:  
{% raw %}{% assign all_categories = pages.products | map: 'category' %}  
{% for item in all_categories %}  
{{ item }}  
{% endfor %}{% endraw %}

Output: 
{% assign all_categories = pages.products | map: 'category' %}
{% for item in all_categories %}  
- {{ item }}  
{%- endfor %}

## Shopify example version

Input:  
{% raw %}{% assign product_titles = example.collection.products | map: 'title' %}  
{{ product_titles | join: ', ' }}{% endraw %}

Output:
{% assign product_titles = example.collection.products | map: 'title' %}
{{ product_titles | join: ', ' }}