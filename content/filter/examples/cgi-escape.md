---
title: cgi_escape
description: CGI escape a string for use in a URL. Replaces any special characters with appropriate %XX replacements. CGI escape normally replaces a space with a plus + sign.
---
Input: {% raw %}**{{ "foo, bar; baz?" | cgi_escape }}**:{% endraw %}

Output: {{ "foo, bar; baz?" | cgi_escape }}