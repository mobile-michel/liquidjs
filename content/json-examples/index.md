---
title: Json examples
description: Contain the content that LiquidJS displays on a page. Objects and variables are displayed when enclosed in double curly braces {{ & }}.
layout: default
override:tags: [index]
date: 2024-01-01
---
{% for item in collections.json %}
- [{{ item.data.title }}]({{ item.url }})
{% endfor %}