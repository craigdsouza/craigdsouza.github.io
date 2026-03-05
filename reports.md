---
layout: default
title: Reports
description: Longer research pieces prepared with the help of AI.
permalink: /reports
---

{% assign placeholders = "diamond,hexagon,square,triangle,circle" | split: "," %}

<div class="page-header">
  <h1>Reports</h1>
  <p>Longer research pieces prepared with the help of AI.</p>
</div>

{% assign sorted_reports = site.reports | sort: "date" | reverse %}
{% if sorted_reports.size > 0 %}
<ul class="post-list">
  {% for report in sorted_reports %}
  {% assign idx = forloop.index0 | modulo: 5 %}
  {% assign placeholder = placeholders[idx] %}
  <li>
    <a href="{{ report.url | relative_url }}" class="post-list-link">
      <img
        src="{% if report.image %}{{ report.image }}{% else %}{{ '/img/placeholders/' | append: placeholder | append: '.svg' | relative_url }}{% endif %}"
        alt=""
        class="post-thumb"
      >
      <div class="post-list-text">
        <span class="post-list-title">{{ report.title }}</span>
        {% if report.description %}
        <div class="post-description">{{ report.description }}</div>
        {% endif %}
        <div class="post-meta">
          {{ report.date | date: "%B %-d, %Y" }}
          {% if report.tags and report.tags.size > 0 %}
            &nbsp;&middot;&nbsp;
            <span class="post-tags">
              {% for tag in report.tags %}<span class="tag">{{ tag }}</span>{% endfor %}
            </span>
          {% endif %}
        </div>
      </div>
    </a>
  </li>
  {% endfor %}
</ul>
{% else %}
<p class="empty-state">Nothing here yet. Check back soon.</p>
{% endif %}
