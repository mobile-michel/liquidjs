---
title: Filters
description:  create the logic and control flow for templates.
layout: default
tags: [primary, footer]
---
{% for item in filters %}
- **[{{ item.name }}](/filter/{{ item.name }}/index.html)** (v{{ item.version }}): {{ item.description }}
{% endfor %}