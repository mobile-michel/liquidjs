---
title: Filters
description: change the output of a Liquid object or variable. They are used within double curly braces {{ & }} and variable assignment. There are separated by a pipe character |.
layout: default
tags: [index, primary]
date: 2024-03-02
---
{% for item in filters %}
- **[{{ item.name | slugify }}]({{ item.name | prepend: '/filter/' | append: '/index.html' | url }})** (v{{ item.version }}): {{ item.description }}
{% endfor %}