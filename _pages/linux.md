---
title: "Linux"
layout: archive
permalink: /linux/
author_profile: true
sidebar:
  nav: "categories"
---

{% assign posts = site.categories.Linux %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
