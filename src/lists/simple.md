---
title: Simple.css
description: repositories with Simple.css
date: 2023-10-04
---
{% for i in github %}
{% if i.css == 'simple.css' %}

{% include 'filter' %}

{% endif %}
{% endfor %}