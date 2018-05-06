---
layout: archive
permalink: /software-security/
title: "Software Security"
author-profile: true
header:
    image: "/assets/images/Security-page-banner.jpg"
---

{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  {% if tag == "Security" %}
    {% for post in posts %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
{% endfor %}