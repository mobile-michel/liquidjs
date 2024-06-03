---
title: Tablerow iteration tag
description: Generates an HTML table. Must be wrapped in opening table> and closing /table> HTML tags.
---
## Basic usage
<table>
{% tablerow product in collection.products %}
  {{ product.title }}
{% endtablerow %}
</table>

## Cols parameter
{% tablerow product in collection.products cols:2 %}
  {{ product.title }}
{% endtablerow %}

## Limit parameter
{% tablerow product in collection.products cols:2 limit:3 %}
  {{ product.title }}
{% endtablerow %}

## Offset parameter
{% tablerow product in collection.products cols:2 offset:3 %}
  {{ product.title }}
{% endtablerow %}

## Range parameter
<!--variable number example-->

{% assign num = 4 %}
<table>
{% tablerow i in (1..num) %}
  {{ i }}
{% endtablerow %}
</table>

<!--literal number example-->

<table>
{% tablerow i in (3..5) %}
  {{ i }}
{% endtablerow %}
</table>