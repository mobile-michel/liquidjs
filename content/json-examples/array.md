---
title: Simple array
description: very simple JSON array
---

### Very simple
**Input**: {% raw %}
{{ array | array_to_sentence_string }}
{% endraw %}
**Output**: {{ array | array_to_sentence_string }}

### For loop
**Input**: {% raw %}
{% for item in array %}
{{ item }}
{% endfor %}
{% endraw %}
**Output**: {% for item in array %}
- {{ item }}
{% endfor %}