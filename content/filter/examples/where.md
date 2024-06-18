---
title: where
description: Creates an array including only the objects with a given property value, or any truthy value by default.
---
In this example, assume you have a list of products and you want to show your *Clover's Apothecary* products separately. Using where, you can create an array containing only the products that have a "type" of "Clover's Apothecary":

Input:  
{% raw %}
{% assign kitchen_products = products.collection.products | where: "vendor", "Clover's Apothecary" %}  
Clover's Apothecary products:  
{% for product in kitchen_products %}  
{{ product.title }}  
{%- endfor %}{% endraw %}

Output:
{% assign kitchen_products = products.collection.products | where: "vendor", "Clover's Apothecary" %}
Clover's Apothecary products:
{% for product in kitchen_products %}
- {{ product.title }}
{%- endfor %}