---
title: newline_to_br
description: Replaces every newline (\n) in a string with an HTML line break (&lt;br />).
---
Input: {% raw %}**{% capture string_with_newlines %}  
Hello  
there  
{% endcapture %}  
{{ string_with_newlines | newline_to_br }}**:{% endraw %}

Output: {% capture string_with_newlines %}
Hello
there
{% endcapture %}

{{ string_with_newlines | newline_to_br }}

HTML code: {{ '<br/>Hello<br/>there<br/>' | url_encode }}