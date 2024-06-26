---
layout: page
title: Energy Committee Projects
permalink: /projects/
menu: Projects
order: d
description: #A growing collection of your cool projects.
display_categories: #[work, fun]
horizontal: false
nav: true
---

## Current Projects
- Town Lighting LED Upgrades
- Solar Arrays
  - Town Office Solar Array Panel
  - School
  - Private Residential Efforts
- Energy Audits of Town Buildings
- Winterization Projects


## Prospective Projects
- Solar arrays
- Energy independence
- Island transportation
- Electric Car Charging Stations

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else if site.enable_projects -%}
<!-- Display projects without categories -->

  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-2">
      {%- for project in sorted_projects -%}
        {% include projects_horizontal.html %}
      {%- endfor %}
      </div>
    </div>
  {%- else -%}
    <div class="grid">
      {%- for project in sorted_projects -%}
        {% include projects.html %}
      {%- endfor %}
    </div>
  {%- endif -%}
{%- endif -%}
</div>
