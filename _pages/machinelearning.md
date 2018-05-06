---
layout: archive
permalink: /machine-learning/
title: "Machine Learning"
author-profile: true
header:
    image: "/assets/images/Machine-learning-page-banner.jpg"
---

{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names and tag == "Machine Learning" %}
  {% assign posts = group_items[forloop.index0] %}
  {% if tag == "Machine Learning" %}
    {% for post in posts %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
{% endfor %}
