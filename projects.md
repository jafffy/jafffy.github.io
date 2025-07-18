---
layout: page
title: Research Projects
permalink: /projects/
---

<div class="projects-grid">
  {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
  {% for project in sorted_projects %}
  <div class="project-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    {% if project.subtitle %}
    <p class="project-subtitle">{{ project.subtitle }}</p>
    {% endif %}
    <p class="project-excerpt">{{ project.excerpt | strip_html | truncatewords: 30 }}</p>
    <div class="project-meta">
      {% if project.period %}
      <span class="period">{{ project.period }}</span>
      {% endif %}
      {% if project.status %}
      <span class="status status-{{ project.status }}">{{ project.status }}</span>
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>

