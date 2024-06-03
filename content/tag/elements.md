---
title: Tags
description:  create the logic and control flow for templates.
layout: default
tags: [primary, footer]
---
{% for item in tags %}
- **[{{ item.name }}](/tag/{{ item.name }}/index.html)** (v{{ item.version }}): {{ item.description }}
{% endfor %}