---
title: GitHub Pages
description: repositories with deploy to GitHub Pages
date: 2023-10-02
---
{% assign number = github | where: 'deploy', 'github-pages' %}
There are {{number.size}} repositories.
{% for i in github %}
{% if i.deploy == 'github-pages' %}

{% include 'filter' %}

{% endif %}
{% endfor %}