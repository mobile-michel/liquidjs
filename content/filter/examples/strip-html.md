---
title: strip_html
description: Removes any HTML tags from a string.
---
Input: {% raw %}**{{ "Have <em>you</em> read <strong>Ulysses</strong>?" | strip_html }}**:{% endraw %}

Output: {{ "Have <em>you</em> read <strong>Ulysses</strong>?" | strip_html }}