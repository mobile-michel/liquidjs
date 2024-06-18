---
title: find_exp
description: Return the first object in an array for which the given expression evaluates to true or return nil if no item in the array satisfies the evaluated expression.
---

Input:  
{% raw %}
{{ product | find: "vendor", "Ted" | json }}{% endraw %}

Output:
```
{{ product | find_exp: "item", "item.vendor == 'Ted'" | json }}
```