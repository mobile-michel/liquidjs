---
title: escape
description: Escapes a string by replacing HTML special characters with escape sequences. It doesn’t change strings that don’t have anything to escape.
---
Input: {% raw %}**{{ "Have you read 'James & the Giant Peach'?" | escape }}**:{% endraw %}

Output: {{ "Have you read 'James & the Giant Peach'?" | escape }}

HTML code: {{ 'Have you read &#39;James &amp; the Giant Peach&#39;?' | strip_html }}

Input: {% raw %}**{{ "Tetsuro Takara" | escape }}**:{% endraw %}

Output: {{ "Tetsuro Takara" | escape }}

HTML code: {% raw %}Tetsuro Takara{% endraw %}