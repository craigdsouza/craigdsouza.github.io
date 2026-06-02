---
layout: default
title: Projects
description: Things I've built and put out into the world.
permalink: /projects
---

{% assign placeholders = "hexagon,triangle,diamond,circle,square" | split: "," %}

<div class="page-header">
  <h1>Projects</h1>
  <p>Things I've built and put out into the world.</p>
</div>

{% assign sorted_projects = site.projects | sort: "date" | reverse %}
{% if sorted_projects.size > 0 %}
<ul class="post-list">
  {% for project in sorted_projects %}
  {% assign idx = forloop.index0 | modulo: 5 %}
  {% assign placeholder = placeholders[idx] %}
  <li>
    <a href="{{ project.url | relative_url }}" class="post-list-link">
      <img
        src="{% if project.image %}{{ project.image }}{% else %}{{ '/img/placeholders/' | append: placeholder | append: '.svg' | relative_url }}{% endif %}"
        alt=""
        class="post-thumb"
      >
      <div class="post-list-text">
        <span class="post-list-title">{{ project.title }}</span>
        {% if project.description %}
        <div class="post-description">{{ project.description }}</div>
        {% endif %}
        <div class="post-meta">
          {{ project.date | date: "%B %-d, %Y" }}
          {% if project.tags and project.tags.size > 0 %}
            &nbsp;&middot;&nbsp;
            <span class="post-tags">
              {% for tag in project.tags %}<span class="tag">{{ tag }}</span>{% endfor %}
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
