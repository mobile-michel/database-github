---
title: Blog
description: This is a blog
layout: base
tags: primary
date: 2023-10-01
pagination:
  data: collections.blog
  size: 10
  alias: items
---

{%- for post in items %}

- [{{ post.data.title }}]({{ post.url }}): {{ post.data.description }}
  {%- endfor %}

{% include 'pagination' %}