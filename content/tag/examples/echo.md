---
title: Echo variable tag
description: Outputs an expression in the rendered HTML. This is identical to wrapping an expression in {{` and `}}, but works inside liquid tags and supports filters.
---
{% assign username = 'Bob' %}
{% echo username | append: ", welcome to LiquidJS!" | capitalize %}