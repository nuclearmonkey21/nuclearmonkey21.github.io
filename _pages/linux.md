---
title: "Linux"
layout: categories
permalink: /linux
author_profile: true
---

{% assign posts = site.categories.Linux %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
