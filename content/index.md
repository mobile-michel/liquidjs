---
title: Home
date: 2024-01-01
layout: default
tags:
  - primary
  - footer
---
{% for item in collections.primary %}
- [{{ item.data.title }}]({{ item.url }})
{% endfor %}