---
layout: page
title: Projects
subtitle: Selected work across robotics, bio, and AI
permalink: /projects
---

<style>
/* Force project thumbnail sizes */
.project-row .thumb img {
  width: 80px !important;
  height: 80px !important;
  max-width: 80px !important;
  max-height: 80px !important;
  object-fit: cover !important;
  border-radius: 8px;
  display: block;
  background: #e5e7eb;
  flex-shrink: 0;
}

@media (max-width: 760px) {
  .project-row .thumb img {
    width: 60px !important;
    height: 60px !important;
    max-width: 60px !important;
    max-height: 60px !important;
  }
}
</style>

{% for item in site.data.projects %}
  {% include portfolio-card.html item=item %}
{% endfor %}
