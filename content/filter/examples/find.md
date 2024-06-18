---
title: find
description: Return the first object in an array for which the queried attribute has the given value or return nil if no item in the array satisfies the given criteria.
---

Input:  
{% raw %}
{{ product | find: "vendor", "Ted" | json }}{% endraw %}

Output:
```
{{ product | find: "vendor", "Ted" | json }}
```