---
title: strip_newlines
description: Removes any newline characters (line breaks) from a string.
---
{% raw %}{% capture string_with_newlines %}  
Hello  
there  
{% endcapture %}  
{{ string_with_newlines | strip_newlines }}{% endraw %}:

{% capture string_with_newlines %}
Hello
there
{% endcapture %}
{{ string_with_newlines | strip_newlines }}