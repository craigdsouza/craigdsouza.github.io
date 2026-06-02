---
layout: default
title: Certifications
description: Courses and certifications I've completed.
permalink: /certifications
---

<div class="page-header">
  <h1>Certifications</h1>
  <p>Courses and certifications I've completed.</p>
</div>

{% for group in site.data.certifications %}
<div class="cert-section">
  <h2 class="cert-category">{{ group.category }}</h2>
  <ul class="cert-list">
    {% for cert in group.items %}
    <li class="cert-item">
      <div class="cert-logo">
        {% if cert.logo %}
        <img src="{{ '/img/issuers/' | append: cert.logo | relative_url }}" alt="{{ cert.issuer }}">
        {% endif %}
      </div>
      <div class="cert-body">
        <span class="cert-title">{{ cert.title }}</span>
        <div class="cert-meta">
          <span class="cert-issuer">{{ cert.issuer }}</span>
          <span class="cert-right">
            {% if cert.date %}<span class="cert-date">{{ cert.date }}</span>{% endif %}
            {% if cert.url %}<a href="{{ cert.url }}" class="cert-link" target="_blank" rel="noopener">↗</a>{% endif %}
          </span>
        </div>
      </div>
    </li>
    {% endfor %}
  </ul>
</div>
{% endfor %}
