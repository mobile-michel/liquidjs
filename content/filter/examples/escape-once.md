---
title: escape_once
description: Escapes a string without changing existing escaped entities. It doesn’t change strings that don’t have anything to escape.
---
Input: {% raw %}**{{ "1 < 2 & 3" | escape_once }}**:{% endraw %}

Output: {{ "1 < 2 & 3" | escape_once }}

HTML code: {{ '1 &lt; 2 &amp; 3' | url_encode }}

Input: {% raw %}**{{ "1 &lt; 2 &amp; 3" | escape_once }}**:{% endraw %}

Output: {{ "1 &lt; 2 &amp; 3" | escape_once }}

HTML code: {{ '1 &lt; 2 &amp; 3' | url_encode }}