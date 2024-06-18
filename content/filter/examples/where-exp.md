---
title: where_exp
description: Select all the objects in an array where the expression is true.
---
In this example, assume you have a list of products and you want to show your kitchen products separately. Using where_exp, you can create an array containing only the products that have a "type" of "kitchen".

Input:  
{% raw %}
{% assign kitchen_products = products.collection.products | where_exp: "item", "item.vendor == 'Polina'" %}
Kitchen products:
{% for product in kitchen_products %}
- {{ product.title }}
{% endfor %}{% endraw %}

Output:
{% assign kitchen_products = products.collection.products | where_exp: "item", "item.vendor == 'Polina'" %}
Kitchen products:
{% for product in kitchen_products %}
- {{ product.title }}
{% endfor %}