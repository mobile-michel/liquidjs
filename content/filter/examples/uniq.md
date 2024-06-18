---
title: uniq
description: Removes any duplicate elements in an array.
---
Input:  
{% raw %}{% assign my_array = "ants, bugs, bees, bugs, ants" | split: ", " %}
{{ my_array | uniq | join: ", " }}{% endraw %}

Output: 
{% assign my_array = "ants, bugs, bees, bugs, ants" | split: ", " %}
{{ my_array | uniq | join: ", " }}