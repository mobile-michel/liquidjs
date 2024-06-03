---
title: Assign variable tag
description: Creates a new variable.
---
{% assign my_variable = false %}
{% if my_variable != true %}
  This statement is valid.
{% endif %}

Wrap a variable value in quotations " to save it as a string.  
{% assign foo = "bar" %}
{{ foo }}