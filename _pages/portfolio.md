---
layout: page
title: Portfolio
permalink: /portfolio/
description: Projecten van Westerveld Bouw — uitbouwen, dakopbouwen, renovaties en meer.
---

<div class="portfolio-grid">
  {% assign featured_projects = site.projects | where: "featured", true %}
  {% assign other_projects = site.projects | where_exp: "p", "p.featured != true" %}
  {% assign ordered_projects = featured_projects | concat: other_projects %}
  {% for project in ordered_projects %}
  <div class="portfolio-card">
    <div class="portfolio-card-image">
      {% if project.cover_image %}
      <img src="{{ project.cover_image | relative_url }}" alt="{{ project.title }}">
      {% endif %}
    </div>
    <div class="portfolio-card-body">
      <p class="category">{{ project.category }}</p>
      <h3>{{ project.title }}</h3>
      <p>{{ project.description | default: project.excerpt | strip_html | truncate: 120 }}</p>
      <a href="{{ project.url | relative_url }}" class="portfolio-card-link">Bekijk project →</a>
    </div>
  </div>
  {% endfor %}
</div>

{% if site.projects.size == 0 %}
<p style="text-align:center; color:#6B7280; padding:3rem 0;">Projecten worden binnenkort toegevoegd.</p>
{% endif %}
