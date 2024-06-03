---
title: Filter cat
description:  create the logic and control flow for templates.
layout: default
tags: [primary, footer]
---
{% for item in filters-category %}
- **{{ item.name }}**: {{ item.description }}
{% endfor %}