---
title: truncatewords
description: Shortens a string down to the number of words passed as an argument. If the specified number of words is less than the number of words in the string, an ellipsis (…) is appended to the string.
---
### Basic usage

{% raw %}**{{ "Ground control to Major Tom." | truncatewords: 3 }}**:{% endraw %}

{{ "Ground control to Major Tom." | truncatewords: 3 }}

### Custom ellipsis

Truncatewords takes an optional second argument that specifies the sequence of characters to be appended to the truncated string. By default this is an ellipsis (…), but you can specify a different sequence.

{% raw %}**{{ "Ground control to Major Tom." | truncatewords: 3, "--" }}**:{% endraw %}

{{ "Ground control to Major Tom." | truncatewords: 3, "--" }}

### No ellipsis

You can avoid showing trailing characters by passing a blank string as the second argument:

{% raw %}**{{ "Ground control to Major Tom." | truncatewords: 3, "" }}**:{% endraw %}

{{ "Ground control to Major Tom." | truncatewords: 3, "" }}