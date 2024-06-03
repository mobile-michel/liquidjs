---
title: Case & when
description: Creates a switch statement to compare a variable with different values. case initializes the switch statement, and when compares its values.
---

{% assign handle = "cake" %}
{% case handle %}
  {% when "cake" %}
     This is a cake
  {% when "cookie", "biscuit" %}
     This is a cookie
  {% else %}
     This is not a cake nor a cookie
{% endcase %}
