---
title: Contents
description: what is LiquidJS template language? It uses a combination of objects, tags, and filters inside template files to display dynamic content.
date: 2024-01-02
layout: default
tags: [primary, footer]
---
{% for item in collections.index %}
- [{{ item.data.title }}]({{ item.url | url }}): {{ item.data.description }}
{% endfor %}