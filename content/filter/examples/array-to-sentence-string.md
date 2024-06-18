---
title: array_to_sentence_string
description: Convert an array into a sentence. Useful for listing tags. Optional argument for connector.
---
{% raw %}**{{ "foo,bar,baz" | split: "," | array_to_sentence_string }}**:{% endraw %}

{{ "foo,bar,baz" | split: "," | array_to_sentence_string }}

{% raw %}**{{ "foo,bar,baz" | split: "," | array_to_sentence_string: "or" }}**:{% endraw %}

{{ "foo,bar,baz" | split: "," | array_to_sentence_string: "or" }}