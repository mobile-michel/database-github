---
title: Astro
description: repositories with Astro
date: 2023-10-03
---
{% assign number = github | where: 'ssg', 'astro' %}
There are {{number.size}} repositories.
{% for i in github %}
{% if i.ssg == 'astro' %}

{% include 'filter' %}

{% endif %}
{% endfor %}