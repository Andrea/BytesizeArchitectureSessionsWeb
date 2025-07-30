---
title: "Posts by Category"
permalink: /categories/
layout: posts
author_profile: true
---


{% include group-by-array collection=site.posts field="categories" %}

{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category | capitalize}}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %} 