---
title: Render file tag
description: Render a Template.
liquidjs: https://liquidjs.com/tags/render.html
shopify: https://shopify.github.io/liquid/tags/template/#render
shopifyDev: https://shopify.dev/docs/api/liquid/tags/render
---
Render a partial template from partials directory specified by partials or root.

{% render 'example.liquid' %}

If extname option is set, the above .liquid extension becomes optional:

{% render 'example' %}

## Variable Scope
When a partial template is rendered, the code inside it can’t access its parent’s variables and its variables won’t be accessible by its parent. This encapsulation makes partials easier to understand and maintain.

## Passing Variables
Variables defined in parent’s scope can be passed to a the partial template by listing them as parameters on the render tag:  
{% assign my_variable = 'apples' %}
{% render 'name', my_variable: my_variable, my_other_variable: 'oranges' %}

globals don’t need to be passed down. They are accessible from all files.

## Outputs & Filters
When filename is specified as literal string, it supports Liquid output and filter syntax. Useful when concatenating strings for a complex filename.  
