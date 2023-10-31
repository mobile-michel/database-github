---
title: Sass & Netlify
description: repositories with a Sass workflow & Netlify deploy
date: 2023-10-02
---
{% for i in github %}
{% if i.sass %} 
{% if i.netlify -%}

{% include 'filter' %}

{% endif %}
{% endif %}
{% endfor %}