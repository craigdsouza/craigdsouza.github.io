---
layout: default
title: Tools
description: Things I've built and put out into the world.
permalink: /tools
---

{% assign placeholders = "hexagon,triangle,diamond,circle,square" | split: "," %}

<div class="page-header">
  <h1>Tools</h1>
  <p>Things I've built and put out into the world.</p>
</div>

{% assign sorted_tools = site.tools | sort: "date" | reverse %}
{% if sorted_tools.size > 0 %}
<ul class="post-list">
  {% for tool in sorted_tools %}
  {% assign idx = forloop.index0 | modulo: 5 %}
  {% assign placeholder = placeholders[idx] %}
  <li>
    <a href="{{ tool.url | relative_url }}" class="post-list-link">
      <img
        src="{% if tool.image %}{{ tool.image }}{% else %}{{ '/img/placeholders/' | append: placeholder | append: '.svg' | relative_url }}{% endif %}"
        alt=""
        class="post-thumb"
      >
      <div class="post-list-text">
        <span class="post-list-title">{{ tool.title }}</span>
        {% if tool.description %}
        <div class="post-description">{{ tool.description }}</div>
        {% endif %}
        <div class="post-meta">
          {{ tool.date | date: "%B %-d, %Y" }}
          {% if tool.tags and tool.tags.size > 0 %}
            &nbsp;&middot;&nbsp;
            <span class="post-tags">
              {% for tag in tool.tags %}<span class="tag">{{ tag }}</span>{% endfor %}
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
