---
title: test one
description: tags from the language category
---
## Inline comment
Anything inside an inline comment tag will not be printed.
{% # this is an inline comment %}
But every line must start with a '#'.
{%
  # this is a comment
  # that spans multiple lines
%}

## Raw
{% raw %}
  In Handlebars, {{ this }} will be HTML-escaped, but
  {{{ that }}} will not.
{% endraw %}

## Comment
Anything you put between {% comment %} and {% endcomment %} tags
is turned into a comment.

## Liquid
{% liquid
  assign names = 'Bob, Sally' | split: ', '

  for name in names
    echo 'Hello, ' | append: name
    unless forloop.last
      echo ', '
    endunless
  endfor
%}

## Echo
{% assign username = 'Bob' %}
{% echo username | append: ", welcome to LiquidJS!" | capitalize %}