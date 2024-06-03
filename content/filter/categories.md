---
title: Filter categories
description: various types like math, string, html, array, date & misc.
layout: default
tags: [index, footer]
date: 2024-03-03
---
{% for item in filters-category %}
- **{{ item.name }}**: {{ item.description }}
{% endfor %}