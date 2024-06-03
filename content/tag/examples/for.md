---
title: for
description: 'Repeats the output of a block of code multiple times.'
layout: default
date: 2024-01-03
---
Example 1
{% for item in objects %}
- {{ item.name }}
{% endfor %}

Example 2
{% for item in objects %}
- {{ item[0] }}: {{ item[1] }}
{% endfor %}