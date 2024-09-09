---
title: Simple object
description: very simple JSON object
---
### Very simple
**Input**: {% raw %}
{{ object.key1 }}
{% endraw %}
**Output**: {{ object.key1 }}

### For loop
**Input**: {% raw %}
{% for item in object %}
- {{ item }}
{% endfor %}
{% endraw %}
**Output**: {% for item in object %}
- {{ item }}
{% endfor %}

### For loop v2
**Input**: {% raw %}
{% for item in object %}
- {{ item[1] }}
{% endfor %}
{% endraw %}
**Output**: {% for item in object %}
- {{ item[1] }}
{% endfor %}