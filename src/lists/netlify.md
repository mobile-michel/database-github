---
title: Netlify
description: repositories with deploy to Netlify
date: 2023-10-02
---
{% for i in github %}
{% if i.netlify %}
- **[{{ i.repo | capitalize }}](https://github.com/mobile-michel/{{ i.repo }})**: {{ i.description }}  
**SSG**: {{i.ssg | capitalize }} - **CSS**: {{i.css}} - **template**: {{i.template | capitalize}} - {% if i.cms %}**CMS**: {{i.cms}}{% endif %}  
{% if i.netlify -%}
**Netlify**: [{{ i.netlify }}](https://{{ i.netlify }}.netlify.app/)
{% endif %}
{% if i.githubPages -%}
**Netlify**: [{{ i.githubPages }}](https://mobile-michel.github.io/{{ i.githubPages }}/)
{% endif %}
{% endif %}
{% endfor %}