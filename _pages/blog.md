---
layout: archive
title: "Writings"
permalink: /blog/
author_profile: true
---

{% include base_path %}

{% for post in site.posts reversed %} {% include archive-single.html %} {% endfor %}
