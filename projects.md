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

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}

.project-card {
  background: #f9fafb;
  border: 1px solid #e5e7eb;
  border-radius: 0.5rem;
  padding: 1.5rem;
  transition: all 0.3s ease;
}

.project-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transform: translateY(-2px);
}

.project-card h3 {
  margin-bottom: 0.5rem;
}

.project-subtitle {
  color: #6b7280;
  font-size: 0.875rem;
  margin-bottom: 0.5rem;
}

.project-excerpt {
  margin-bottom: 1rem;
}

.project-meta {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 0.875rem;
}

.period {
  color: #6b7280;
}

.status {
  padding: 0.25rem 0.75rem;
  border-radius: 0.25rem;
  font-weight: 500;
  font-size: 0.75rem;
}

.status-active {
  background: #d1fae5;
  color: #065f46;
}

.status-completed {
  background: #dbeafe;
  color: #1e40af;
}
</style>