---
title: Home
description: what is LiquidJS template language? It uses a combination of objects, tags, and filters inside template files to display dynamic content.
date: 2024-01-01
layout: default
tags: [primary, footer]
---
{% for item in collections.index %}
- [{{ item.data.title }}]({{ item.url | url }}): {{ item.data.description }}
{% endfor %}

## Interesting links
- [LiquidJS](https://liquidjs.com/), this version.
- [Liquid on Shopify](https://shopify.github.io/liquid/), the open-source template language.
- [The Shopify Cheat Sheet](https://www.shopify.com/partners/shopify-cheat-sheet)
- [Shopify API reference docs](https://shopify.dev/docs/api), with all the proprietary objects.