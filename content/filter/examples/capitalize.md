---
title: capitalize
description: Makes the first character of a string capitalized.
---
**{% raw %}{{ "title" | capitalize }}{% endraw %}**: {{ "title" | capitalize }}

`Capitalize` only capitalizes the first character of a string, so later words are not affected (not right!!!):

**{% raw %}{{ "my great Title" | capitalize }}{% endraw %}**: {{ "my great Title" | capitalize }}