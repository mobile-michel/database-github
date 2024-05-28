---
title: Repos details
description: GitHub repositories with details
layout: base
tags: primary
date: 2023-10-03
---
{% for i in github %}
- **[{{ i.github | capitalize }}](https://github.com/mobile-michel/{{ i.github }})**: {{ i.description }}
**SSG**: {{i.ssg | capitalize }} - **CSS**: {{i.css}} - **template**: {{i.template | capitalize}} - {% if i.cms %}**CMS**: {{i.cms}}{% endif %}
{% if i.netlify -%}
**Netlify**: [{{ i.netlify }}](https://{{ i.netlify }}.netlify.app/)
{% endif %}
{%- if i.githubPages -%}
**GitHub Pages**: [{{ i.githubPages }}](https://mobile-michel.github.io/{{ i.githubPages }}/)
{% endif %}
{% endfor %}