---
title: Categories
description: list of repo categories
---
{% assign categories = github | map: "category" | uniq %}
{% for i in categories %}
- {{ i }}
{% endfor %}