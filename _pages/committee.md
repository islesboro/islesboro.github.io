---
layout: page
permalink: /committee/
title: Islesboro Energy Committee
menu: Committee
order: e
description: #x
nav: true
---

## Mission Statement
To explore ideas and develop proposals to present to the Select Board of the Town of Islesboro relating to the best options that address the energy needs of the Town.  The ideas and proposals will be made available to support efforts toward sustainability across the entire island community.

<br />

## Members

<div class="row">
    <div class="col-sm mt-2 mt-md-0">
Myra Sinnott (Interim Chair)
<br />
Bill Thomas (Vice Chair)
<br />
Harriet Bering
<br />
J. Cressica Brazier
<br />
Dick DeGrasse
    </div>
    <div class="col-sm mt-2 mt-md-0">
Holly Fields
<br />
Josh Leach
<br />
Toby Martin
<br />
Monica Mullins
<br />
Melissa Burns (Ex Officio)
    </div>
</div>
<br />

<div class="row">
    <div class="col-sm mt-2 mt-md-0">
<h2>Current Projects</h2>
<ul>
  <li>Community clean energy and energy efficiency planning for DOE Rural Energy Prize</li>
  <li>Town Building energy upgrades</li>
  <ul>
    <li>Energy Audits</li>
    <li>LED Lighting for Town Office and Library</li>
    <li>Insulation for Town Office and Library</li>
    <li>Electric Vehicle Charger at Town Office</li>
  </ul>
  <li>Solar Arrays</li>
  <ul>
    <li>Town Office (46kW)</li>
    <!--/li>  - School (65kW)</li-->
    <li>Transfer Station Salt Shed Array (30kW)</li>
  </ul>
</ul>
    </div>
    <div class="col-sm mt-2 mt-md-0">
<h2>Prospective Projects</h2>
<ul>
  <li>Cooperative solar arrays and other clean energy projects</li>
  <li>Energy independence and microgrids</li>
  <li>Building electrification of Town Office and Library</li>
</ul>
    </div>
</div>

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