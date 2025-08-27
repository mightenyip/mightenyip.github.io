---
layout: single
title: "Projects"
permalink: /projects/
classes: wide
---

A selection of academic, startup, and translational work.

{% raw %}{% assign projects = site.projects | sort: 'title' %}

<div class="feature__wrapper">
  {% for project in projects %}
    <div class="feature__item">
      <div class="archive__item">
        {% if project.header.teaser %}
          <div class="archive__item-teaser">
            <img src="{{ project.header.teaser }}" alt="{{ project.title }}">
          </div>
        {% endif %}
        <div class="archive__item-body">
          <h3 class="archive__item-title">
            <a href="{{ project.url }}">{{ project.title }}</a>
          </h3>
          <div class="archive__item-excerpt">
            <p>{{ project.excerpt }}</p>
          </div>
          {% if project.tags %}
            <div class="archive__item-tags">
              {% for tag in project.tags %}
                <span class="badge badge--primary">{{ tag }}</span>
              {% endfor %}
            </div>
          {% endif %}
        </div>
      </div>
    </div>
  {% endfor %}
</div>{% endraw %}
