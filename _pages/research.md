---
layout: page
title: Research
permalink: /research/
description: 
nav: true
nav_order: 1
display_categories: [work, fun]
horizontal: false
---

*<u>Keywords:</u> multi-robot systems, cooperative robot control, human-multi-robot collaboration, cooperative manipulation, control of multi-agent systems, control of mobile robots.*

My research is about the modeling, control design, and analysis of **multi-robot systems**. The main objective is to make groups of autonomous robots cooperate in order to reach a disered behavior or carry out a specific task while dealing with the specific challenges of multi-robot systems such as limited and local information and physical/interaction constraints.

My current research is focused on four main subjects:

* Multi-objective control of **heterogeneous** robotic teams
* Shared control for **human-multi-robot collaboration**
* **Open multi-robot systems** for resilience
* **Synchronization and topology identification** of cooperative multi-agent systems

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
