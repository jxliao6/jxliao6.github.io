---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% include base_path %} -->

<h2>First-author main projects</h2>
{% for post in site.publications reversed %}
  {% if post.mainproject == 'true'%}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}



<h2>Others</h2>
{% for post in site.publications reversed %}
  {% if post.mainproject == 'false' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
