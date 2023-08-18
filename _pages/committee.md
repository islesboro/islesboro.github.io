---
layout: page
permalink: /committee/
title: Islesboro Energy Committee
menu: Committee
order: e
description: #Materials for courses you taught. Replace this text with your description. s
nav: true
---

## Mission Statement
To explore ideas and develop proposals to present to the Select Board of the Town of Islesboro relating to the best options that address the energy needs of the Town.  The ideas and proposals will be made available to support efforts toward sustainability among the entire island community.

<br />

## Members

Myra Sinnott (Interim Chair)

Bill Thomas (Vice Chair)

Holly Fields

Toby Martin (Treasurer)

Dick DeGrasse

J. Cressica Brazier

Josh Leach

Harriet Bering

Monica Mullins

Melissa Burns (Ex Officio)

<br />


## Current Projects
- Community clean energy and energy efficiency planning for DOE Rural Energy Prize
- Town Building energy upgrades
  - Energy Audits
  - LED Lighting for Town Office and Library
  - Insulation for Town Office and Library
  - Electric Vehicle Charger at Town Office
- Solar Arrays
  - Town Office (46kW)
  - School (65kW)
  - Transfer Station Salt Shed Array (30kW)

<br />

## Prospective Projects
- Cooperative solar arrays and other clean energy projects
- Energy independence
- Island transportation
- Electric Vehicle Charging Stations

<br />

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

{%- else -%}
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