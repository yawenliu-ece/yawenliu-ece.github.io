---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% comment %} Separate publications into two categories {% endcomment %}
{% assign conference_papers = "" | split: "" %}
{% assign poster_demos = "" | split: "" %}
{% for post in site.publications %}
  {% if post.pub_type == 'poster' or post.pub_type == 'demo' %}
    {% assign poster_demos = poster_demos | push: post %}
  {% else %}
    {% assign conference_papers = conference_papers | push: post %}
  {% endif %}
{% endfor %}

{% comment %} Conferences and Journal Papers section {% endcomment %}
<h2 class="archive__subtitle">Conferences and Journal Papers</h2>

{% for post in conference_papers reversed %}
  {% include archive-single.html %}
{% endfor %}

{% comment %} Poster and Demo section {% endcomment %}
{% if poster_demos.size > 0 %}
  <h2 class="archive__subtitle">Poster and Demo</h2>

  {% for post in poster_demos reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}
