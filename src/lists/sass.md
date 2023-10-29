---
title: Sass & Netlify
description: repositories with a Sass workflow & Netlify deploy
date: 2023-10-02
---
{% for i in github %}
{% if i.sass %} 
{% if i.netlify -%}
- **[{{ i.repo | capitalize }}](https://github.com/mobile-michel/{{ i.repo }})**: {{ i.description }}  
**SSG**: {{i.ssg | capitalize }} - **CSS**: {{i.css}} - **template**: {{i.template | capitalize}} - {% if i.cms %}**CMS**: {{i.cms}}{% endif %} 
**Netlify**: [{{ i.netlify }}](https://{{ i.netlify }}.netlify.app/)
{% if i.githubPages -%}
**Netlify**: [{{ i.githubPages }}](https://mobile-michel.github.io/{{ i.githubPages }}/)
{% endif %}
{% endif %}
{% endif %}
{% endfor %}