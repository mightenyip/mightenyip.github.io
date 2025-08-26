---
layout: page
title: Projects
subtitle: Selected work across robotics, bio, and AI
permalink: /projects
---

{% for item in site.data.projects %}
  {% include portfolio-card.html item=item %}
{% endfor %}
