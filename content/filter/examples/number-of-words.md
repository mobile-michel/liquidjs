---
title: number_of_words
description: Count the number of words in some text.
---
This filter takes an optional argument to control the handling of Chinese-Japanese-Korean (CJK) characters in the input string:

- passing 'cjk' as the argument will count every CJK character detected as one word irrespective of being separated by whitespace.
- passing 'auto' (auto-detect) works similar to 'cjk' but is more performant if the filter is used on a variable string that may or may not contain CJK chars.

{% raw %}**{{ "Hello world!" | number_of_words }}**:{% endraw %}

{{ "Hello world!" | number_of_words }}

{% raw %}**{{ "你好hello世界world" | number_of_words }}**:{% endraw %}

{{ "你好hello世界world" | number_of_words }}

{% raw %}**{{ "你好hello世界world" | number_of_words: "cjk" }}**:{% endraw %}

{{ "你好hello世界world" | number_of_words: "cjk" }}

{% raw %}**{{ "你好hello世界world" | number_of_words: "auto" }}**:{% endraw %}

{{ "你好hello世界world" | number_of_words: "auto" }}