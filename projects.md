---
layout: default
title: "Projects"
---

# Projects

> **Note:** This page is a work in progress.

{% if site.projects.size > 0 %}
<div class="project-list">
  {% for project in site.projects %}
  <div class="project-item">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    
    {% if project.description %}
    <p>{{ project.description }}</p>
    {% endif %}
    
    <div class="project-links">
      {% if project.github %}
      <a href="{{ project.github }}" target="_blank">🔗 GitHub</a>
      {% endif %}
      
      {% if project.paper %}
      <a href="{{ project.paper }}" target="_blank">📄 Paper</a>
      {% endif %}
      
      {% if project.blog %}
      <a href="{{ project.blog | relative_url }}">✍️ Blog Post</a>
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>
{% else %}
<p>No projects yet. Check back soon!</p>
{% endif %}