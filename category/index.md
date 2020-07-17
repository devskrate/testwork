---
layout: minimal
title: Tags
---

<div class="tags">
  {% assign category_list = site.category %}
      {% for category in category_list %}
          <a id = "tag" href="{{site.url}}/category/{{category}}">{{ category }}</a>
      {% endfor %}
  {% assign tags_list = nil %}
</div>