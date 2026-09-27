---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
---

## Profile

Computer vision and edge AI engineer focused on visual localization, foundation-model perception, embedded inference, and engineering tools that make experiments reproducible.

## Education

- **B.S. in Computer Engineering**, Seokyeong University — Seoul, South Korea

## Research and engineering experience

### Korea Electronics and Telecommunications Research Institute (ETRI)

Research engineering across GNSS-denied UAM visual localization, aerial-image retrieval, foundation-model features, metadata filtering, local matching, and edge deployment.

### Multimodal time-series research

Designed text/video preprocessing and cross-modal attention interfaces, and continue to investigate facial-coordination signals as a technical representation-learning problem.

### Graduation capstone — Safe Landing for UAV Delivery

Ongoing simulation-based system using DINOv2, RGB-D, ROS 2, and Gazebo. The project is explicitly not presented as real-flight experience.

## Technical skills

**Vision & ML:** DINOv2, DINOv3, VPR, FAISS, LightGlue, ONNX Runtime, object detection, image segmentation

**Edge & systems:** Jetson AGX Orin, Raspberry Pi 5, Hailo-10H, profiling, model conversion, deployment validation

**Software:** Python, C#, .NET, WPF, Django, Spring Boot, AWS, CI/CD, ROS 2, Gazebo

## Publications

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
