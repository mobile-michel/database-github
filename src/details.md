---
title: Repos details
description: GitHub repositories with details
layout: base
tags: primary
date: 2023-10-03
---
{% for element in github %}
{% assign item = element | group_by: 'category' %}
<p>{{ item.category }}</p>
<ul>
    {% for item in element.items %}
    <li><a href="{{ item.link }}">{{ item.id }}</a>: {{ item.idDescription }}</li>
    {% endfor %}
</ul>
{% endfor %}

{% for i in github %}
- **{{ i.github | capitalize }}**: {{ i.description }} | [GitHub repo]({{ i.github }}) | [Deploy](https://{{ i.url }}/)  
**site generator**: {{i.ssg | capitalize }} | **stylesheet**: {{i.css}} | **template**: {{i.template | capitalize}} {% if i.sass %} |**Sass**{% endif %} {% if i.cms %} |**DecapCMS**{% endif %}
{% endfor %}
