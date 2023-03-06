---
title: "Blog"
layout: archive
permalink: /blog/
author_profile: true
sidebar:
  nav: "categories"
---

{% assign posts = site.categories.Blog %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
