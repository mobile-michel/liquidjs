---
title: url_decode
description: Decodes a string that has been encoded as a URL.
---
Input: {% raw %}**{{ "%27Stop%21%27+said+Fred" | url_decode }}**:{% endraw %}

Output: {{ "%27Stop%21%27+said+Fred" | url_decode }}