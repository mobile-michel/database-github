---
title: Netlify
description: repositories with deploy to Netlify
date: 2023-10-02
---
{% for i in github %}
{% if i.netlify %}

{% include 'filter' %}

{% endif %}
{% endfor %}