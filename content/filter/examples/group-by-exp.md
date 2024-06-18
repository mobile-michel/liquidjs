---
title: group_by_exp
description: Group an array’s items using a Liquid expression.
---

Input:  
{% raw %}
{{ product | group_by_exp: "item", "item.vendor | truncate: 3, ''" | json: 2 }}{% endraw %}

Output:
```
{{ product | group_by_exp: "item", "item.vendor | truncate: 3, ''" | json: 2 }}
```