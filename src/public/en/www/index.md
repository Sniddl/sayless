---
title: Say Less
suggestions: false
eleventyExcludeFromCollections:
  - {{ locale }}
---

# Topics
{%- assign suggestions = collections[locale] | alphabetic -%}
{% for page in suggestions %}
  * [{{ page.data.title }}]({{ page | toUrl }})
{%- endfor %}
