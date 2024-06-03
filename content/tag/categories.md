---
title: Tag categories
description: various types like iteration, control flow, variable, file & language.
layout: default
tags: [index, footer]
date: 2024-02-03
---
{% for item in tags-category %}
- **{{ item.name }}**: {{ item.description }}
{% endfor %}