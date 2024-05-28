---
title: All GitHub repos
description: list of all GitHub repositories
layout: base
tags: primary
date: 2023-10-04
---
There are {{ github.size }} GitHub repositories.
{% for i in github %}
- **{{ i.category }}**: [{{ i.github | capitalize }}](https://{{ i.url }}) | [Github repo](https://github.com/mobile-michel/{{ i.github }})
{% endfor %}