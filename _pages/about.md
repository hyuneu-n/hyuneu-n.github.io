---
permalink: /
title: "Computer Vision & Edge AI Engineer"
author_profile: true
---

I build computer-vision systems that connect research ideas to deployable software. My work spans GNSS-denied visual localization, foundation-model perception, edge inference, and validation tooling.

<div class="home__metrics">
  <span>Visual localization</span>
  <span>Edge deployment</span>
  <span>ROS 2 / Gazebo</span>
  <span>C# / .NET</span>
</div>

## Selected engineering work

{% assign featured_projects = site.portfolio | where: "featured", true %}
<div class="project-grid">
{% for project in featured_projects %}
  <article class="project-card">
    <p class="project-card__eyebrow">{{ project.role }}</p>
    <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
    <p>{{ project.excerpt }}</p>
    <p class="project-card__stack">{{ project.stack }}</p>
  </article>
{% endfor %}
</div>

## Research direction

At ETRI, I worked on aerial-image retrieval and matching for UAM localization in GNSS-denied environments, including edge deployment and latency investigation. Alongside vision localization, I am continuing multimodal time-series research that combines text, video, and facial coordination signals. My current capstone extends foundation-model perception into a ROS 2/Gazebo safe-landing system; it is a simulation-based engineering project, not a claim of real-flight deployment.

<p><a class="btn btn--primary" href="{{ '/projects/' | relative_url }}">View projects</a> <a class="btn btn--inverse" href="{{ '/cv/' | relative_url }}">View CV</a></p>
