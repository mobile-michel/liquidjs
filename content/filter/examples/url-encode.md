---
title: url_encode
description: Converts any URL-unsafe characters in a string into percent-encoded characters.
---
Input: {% raw %}**{{ "john@liquid.com" | url_encode }}**:{% endraw %}

Output: {{ "john@liquid.com" | url_encode }}

Input: {% raw %}**{{ "Tetsuro Takara" | url_encode }}**:{% endraw %}

Output: {{ "Tetsuro Takara" | url_encode }}