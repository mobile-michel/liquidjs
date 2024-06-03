---
title: Tag cat
description:  create the logic and control flow for templates.
layout: default
tags: [primary, footer]
---
{% for item in tags-category %}
- **{{ item.name }}**: {{ item.description }}
{% endfor %}