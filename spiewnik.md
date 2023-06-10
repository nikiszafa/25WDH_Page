---
layout: page
title: Śpiewnik
permalink: /piosenki/
---

<div class="list-group">
  {% for page in site.piosenki %}
 <a href="{{ page.url }}" class="list-group-item list-group-item-action">
    <div class="d-flex w-100 justify-content-between">
      <h5 class="mb-1">{{ page.title }}</h5>
      <small>{{ page.date | date: "%Y-%m-%d" }}</small>
    </div>
    <p class="mb-1">{{ page.description }}</p>
  </a>
  {% endfor %}

</div>
