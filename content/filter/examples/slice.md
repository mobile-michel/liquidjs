---
title: slice
description: Returns a substring of 1 character beginning at the index specified by the first argument. An optional second argument specifies the length of the substring to be returned. String indices are numbered starting from 0.
---
Input: {% raw %}**{{ "Liquid" | slice: 0 }}**:{% endraw %}

Output: {{ "Liquid" | slice: 0 }}

Input: {% raw %}**{{ "Liquid" | slice: 2 }}**:{% endraw %}

Output: {{ "Liquid" | slice: 2 }}

Input: {% raw %}**{{ "Liquid" | slice: 2, 5 }}**:{% endraw %}

Output: {{ "Liquid" | slice: 2, 5 }}

If the first argument is a negative number, the indices are counted from the end of the string:

Input: {% raw %}**{{ "Liquid" | slice: -3, 2 }}**:{% endraw %}

Output: {{ "Liquid" | slice: -3, 2 }}