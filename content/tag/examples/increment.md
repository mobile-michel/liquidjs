---
title: Increment variable tag
description: Creates a new number variable, and increases its value by one every time it is called. The first value is 0.
---
{% increment my_counter %}  
{% increment my_counter %}  
{% increment my_counter %}

Variables created through the increment tag are independent from variables created through assign or capture.

In the example below, a variable named “var” is created through assign. The increment tag is then used several times on a variable with the same name. Note that the increment tag does not affect the value of “var” that was created through assign.

{% assign var = 10 %}  
{% increment var %}  
{% increment var %}  
{% increment var %}  
{{ var }}