---
layout: page
title: News
menu: News
permalink: /news/
order: c
description: #Materials for courses you taught. Replace this text with your description.
nav: true
---

## News
          
<div class="news">
  {% if site.news != blank -%} 
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
    {%- assign news = site.news | reverse -%} 
    {% for item in news %} 
      <tr>
        <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
        <td>
          {% if item.inline -%} 
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
          {%- else -%} 
            <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
          {%- endif %} 
        </td>
      </tr>
    {%- endfor %} 
    </table>
  </div>
{%- else -%} 
  <p>No news so far...</p>
{%- endif %} 
</div>

<br />