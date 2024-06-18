---
title: slugify
description: Convert a string into a lowercase URL “slug”.
---
Input: {% raw %}**{{ "The _cönfig.yml file" | slugify }}**:{% endraw %}

Output: {{ "The _cönfig.yml file" | slugify }}

Input: {% raw %}**{{ "The _cönfig.yml file" | slugify: "pretty" }}**:{% endraw %}

Output: {{ "The _cönfig.yml file" | slugify: "pretty" }} **(works, but not like the doc !!!)**

Input: {% raw %}**{{ "The _cönfig.yml file" | slugify: "ascii" }}**:{% endraw %}

Output: {{ "The _cönfig.yml file" | slugify: "ascii" }} **(works, but not like the doc !!!)**

Input: {% raw %}**{{ "The cönfig.yml file" | slugify: "latin" }}**:{% endraw %}

Output: {{ "The cönfig.yml file" | slugify: "latin" }} **(works, but not like the doc !!!)**

Input: {% raw %}**{{ "The cönfig.yml file" | slugify: "latin", true }}**:{% endraw %}

Output: {{ "The cönfig.yml file" | slugify: "latin", true }} **(works, but not like the doc !!!)**