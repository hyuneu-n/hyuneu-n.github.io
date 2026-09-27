---
title: "Engineering Projects"
permalink: /projects/
layout: archive
author_profile: true
---

Systems I have designed, implemented, or evaluated across computer vision, edge inference, robotics simulation, and software tooling.

{% assign projects = site.portfolio | sort: "order" %}
<div class="project-grid project-grid--archive">
{% for project in projects %}
  <article class="project-card">
    <p class="project-card__eyebrow">{{ project.role }}</p>
    <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
    <p>{{ project.excerpt }}</p>
    <p class="project-card__stack">{{ project.stack }}</p>
    <a class="project-card__link" href="{{ project.url | relative_url }}">Read case study →</a>
  </article>
{% endfor %}
</div>
