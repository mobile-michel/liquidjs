---
title: uri_escape
description: Percent encodes any special characters in a URI. URI escape normally replaces a space with %20. Reserved characters will not be escaped.
---
Input: {% raw %}**{{ "https://example.com/?q=foo, \bar?" | uri_escape }}**:{% endraw %}

Output: {{ "https://example.com/?q=foo, \bar?" | uri_escape }}