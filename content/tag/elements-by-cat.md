---
title: Tags by cat
description: Create the logic and control flow for templates. The curly brace percentage delimiters {% & %} and the text that they surround do not produce any visible output when the template is rendered. This lets you assign variables and create conditions or loops without showing any of the LiquidJS logic on the page.
layout: default
tags: [index, primary]
date: 2024-02-02
---

{% for item in tag %}
{% assign item = item.category %}
- {{ item }}
{% endfor %}