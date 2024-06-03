---
title: Liquid language tag
description: Encloses multiple tags within one set of delimiters, to allow writing Liquid logic more concisely.
---
{% liquid
  assign names = 'Bob, Sally' | split: ', '

  for name in names
    echo 'Hello, ' | append: name
    unless forloop.last
      echo ', '
    endunless
  endfor
%}