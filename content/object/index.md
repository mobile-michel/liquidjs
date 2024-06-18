---
title: Objects
description: Contain the content that LiquidJS displays on a page. Objects and variables are displayed when enclosed in double curly braces {{ & }}.
layout: default
tags: [index, primary, footer]
date: 2024-01-01
---
{% for item in objects %}
- **{{ item.name }}**: {{ item.description }} (example: {{ item.example }}).
{% endfor %}