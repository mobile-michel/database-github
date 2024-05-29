---
title: Sass
description: repositories with a Sass workflow
date: 2023-10-02
---
{% assign number = github | where: 'sass' %}
There are {{number.size}} repositories.
{% for i in github %}
{% if i.sass == true %} 
{% include 'filter' %}
{% endif %}
{% endfor %}