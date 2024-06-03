---
title: If, elsif & else control flow tag
description: Executes a block of code only if a certain condition is true.
product:
    title: Awesome Shoes
customer:
    name: anonymous
---
## If
{% if product.title == "Awesome Shoes" %}
  These shoes are awesome!
{% endif %}

## Elsif / else
Adds more conditions within an if or unless block.  
<!-- If customer.name = "anonymous" -->
{% if customer.name == "kevin" %}
  Hey Kevin!
{% elsif customer.name == "anonymous" %}
  Hey Anonymous!
{% else %}
  Hi Stranger!
{% endif %}