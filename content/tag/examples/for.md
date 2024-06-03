---
title: For iteration tag
description: Iteration tags run blocks of code repeatedly.
---
## Basic usage
### For...in
{% for product in collection.products %}
  {{ product.title }}
{% endfor %}

For loops can iterate over arrays, hashes, and ranges of integers. When iterating a hash, item[0] contains the key, and item[1] contains the value:  
