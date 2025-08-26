---
layout: page
title: Projects
subtitle: Selected work across robotics, bio, and AI
permalink: /projects
---

<div class="projects-grid">
  {% for item in site.data.projects %}
    {% include portfolio-card.html item=item %}
  {% endfor %}
</div>
