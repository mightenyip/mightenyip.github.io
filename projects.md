---
layout: single
title: "Projects"
subtitle: "Selected work across robotics, bio, and AI"
permalink: /projects/
classes: wide
---

<style>
/* Force project thumbnail sizes with maximum specificity */
.project-thumbnail,
.project-row .thumb img,
body .project-row .thumb img,
body .page .project-row .thumb img,
div.project-row div.thumb img,
body div.project-row div.thumb img,
body .page div.project-row div.thumb img,
.project-row .thumb > img,
body .project-row .thumb > img {
  width: 80px !important;
  height: 80px !important;
  max-width: 80px !important;
  max-height: 80px !important;
  object-fit: cover !important;
  border-radius: 8px !important;
  display: block !important;
  background: #e5e7eb !important;
  flex-shrink: 0 !important;
  box-sizing: border-box !important;
}

@media (max-width: 760px) {
  .project-thumbnail,
  .project-row .thumb img,
  body .project-row .thumb img,
  body .page .project-row .thumb img,
  div.project-row div.thumb img,
  body div.project-row div.thumb img,
  body .page div.project-row div.thumb img,
  .project-row .thumb > img,
  body .project-row .thumb > img {
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
