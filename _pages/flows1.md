---
layout: archive
permalink: /microsoft-flows/
title: "El sublime arte de no programar"
author_profile: true
header: 
    image: "/images/IMG_20180811_102208.jpg"
---
{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
  {% endfor %}
{% endfor %}