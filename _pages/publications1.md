---
layout: archive
title: "Publications"
permalink: /publications1/
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my articles on <u><a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</u> and some of my prototypes on <u><a href="{{site.author.youtube}}">my YouTube list</a>
{% endif %}

<!-- {% include base_path %} -->

<h2>Conference Regular Papers and Journal Papers</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'regular' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}



<h2>Conference Late Breaking Work, Workshop Papers, Posters, Demos</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'short' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
