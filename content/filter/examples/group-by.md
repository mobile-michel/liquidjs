---
title: group_by
description: Group an array’s items by a given property.
---

Input:  
{% raw %}
{{ product | group_by: "vendor" | json: 2 }}{% endraw %}

Output:
```
{{ product | group_by: "vendor" | json: 2 }}
```