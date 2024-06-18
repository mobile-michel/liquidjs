---
title: xml_escape
description: Escape some text for use in XML.
---
Input: {% raw %}**{{ "Have you read \'James & the Giant Peach\'?" | xml_escape }}**:{% endraw %}

Output: {{ "Have you read \'James & the Giant Peach\'?" | xml_escape }}

HTML code: {{ 'Have you read &#39;James &amp; the Giant Peach&#39;?' | url_encode }}