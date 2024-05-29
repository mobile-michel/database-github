---
title: Decap CMS
description: repositories with Decap CMS
date: 2023-10-10
---
{% assign number = github | where: 'cms' %}
There are {{number.size}} repositories.
{% for i in github %}
{% if i.cms == true %}

{% include 'filter' %}

{% endif %}
{% endfor %}