---
title: Filters
description: GitHub repositories filtered
layout: base
tags: primary
date: 2023-10-02
---
{% for i in collections.list %}
- [{{i.data.title}}]({{i.url}}): {{i.data.description}}
{% endfor %}