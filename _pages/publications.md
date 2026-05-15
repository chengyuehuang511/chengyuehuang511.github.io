---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
---

{% include base_path %}

<div class="publication-list">
  {% for post in site.publications reversed %}
    {% include publication-row.html %}
  {% endfor %}
</div>
