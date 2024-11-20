---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% include base_path %} -->

<h2>First-author full paper and workshop</h2>
{% for post in site.publications reversed %}
  {% if post.mainproject == 'true'%}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}



<h2>Other full paper</h2>
{% for post in site.publications reversed %}
  {% if post.mainproject == 'false' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
