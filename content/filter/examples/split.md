---
title: split
description: Divides a string into an array using the argument as a separator. Split is commonly used to convert comma-separated items from a string to an array.
---
{% raw %}{% assign beatles = "John, Paul, George, Ringo" | split: ", " %}  
{% for member in beatles %}  
  {{ member }}  
{% endfor %}{% endraw %}: 

{% assign beatles = "John, Paul, George, Ringo" | split: ", " %}
{% for member in beatles %}
  {{ member }}
{% endfor %}