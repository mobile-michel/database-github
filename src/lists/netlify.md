---
title: Netlify
description: repositories with deploy to Netlify
date: 2023-10-02
---
{% assign number = github | where: 'deploy', 'netlify' %}
There are {{number.size}} repositories.
{% for i in github %}
{% if i.deploy == 'netlify' %}

{% include 'filter' %}

{% endif %}
{% endfor %}