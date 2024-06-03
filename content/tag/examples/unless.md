---
title: Unless control flow tag
description: The opposite of if, executes a block of code only if a certain condition is not met.
product:
    title: Terrible Shoes
customer:
    name: anonymous
---
{% unless product.title == "Awesome Shoes" %}
  These shoes are not awesome.
{% endunless %}

This would be the equivalent of doing the following:  
{% if product.title != "Awesome Shoes" %}
  These shoes are not awesome.
{% endif %}