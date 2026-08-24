---
layout: page
title: Open positions
permalink: /positions/
description: Open research positions in the Rainbow team
nav: true
nav_order: 6
display_categories: [PhD, Master thesis]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_positions = site.positions | where: "category", category %}
  {% assign sorted_positions = categorized_positions | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for position in sorted_positions %}
      {% include positions_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for position in sorted_positions %}
      {% include positions.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_positions = site.positions | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for position in sorted_positions %}
      {% include positions_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for position in sorted_ppositions %}
      {% include positions.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
