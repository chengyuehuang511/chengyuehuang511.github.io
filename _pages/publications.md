---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
wide_archive: true
---

{% include base_path %}

<div class="publication-list">
  {% assign current_year = "" %}
  {% for post in site.publications reversed %}
    {% assign post_year = post.date | date: "%Y" %}
    {% if post_year != current_year %}
      <h2 class="publication-year">{{ post_year }}</h2>
      {% assign current_year = post_year %}
    {% endif %}
    {% include publication-row.html post=post %}
  {% endfor %}
</div>
