---
layout: archive
permalink: /blog/
title: "Blog"
author_profile: true
---

Welcome to our blog! Here we share stories from our adventures, life updates, and everything in between. From travel tales to everyday moments, this is where we document our journey together.

{% include base_path %}

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  <p style="text-align: center; color: #999; font-style: italic; padding: 40px 0;">No posts yet — check back soon for our latest adventures! ✈️</p>
{% endif %}