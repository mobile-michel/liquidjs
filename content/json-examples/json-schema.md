---
title: JSON Schema
description: complex JSON schema
---
### Version 1
**Input**: {% raw %}
{{ json-schema.first_name }}
{% endraw %}
**Output**: {{ json-schema.first_name }}

### Version 2
**Input**: {% raw %}
{{ json-schema.address.city }}
{% endraw %}
**Output**: {{ json-schema.address.city }}