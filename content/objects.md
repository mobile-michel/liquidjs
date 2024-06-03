---
title: Objects
description: contain the content that Liquid displays on a page.
layout: default
tags: [primary, footer]
---
{% for item in objects %}
- **{{ item.name }}**: {{ item.description }} (example: {{ item.example }}).
{% endfor %}