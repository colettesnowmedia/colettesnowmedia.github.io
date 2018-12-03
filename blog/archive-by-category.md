---
layout: page
title: Archive - By Category
---

{%- for cat in site.cats -%}

## {{ cat.title }}

{% for post in site.categories[cat.term] -%}
* {{ post.date | date: "%d/%m" }}: [{{- post.title -}}]({{- post.url -}})
{% endfor %}

{% endfor %}