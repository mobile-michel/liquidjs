---
title: Inline comment language tag
description: Add comments to a Liquid template using an inline tag. Text enclosed in an inline comment tag will not be printed.
---
Anything inside an inline comment tag will not be printed.
{% # this is an inline comment %}
But every line must start with a '#'.
{%
  # this is a comment
  # that spans multiple lines
%}
