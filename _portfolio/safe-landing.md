---
title: "Vision-Based Safe Landing in Simulation"
collection: portfolio
permalink: /projects/safe-landing/
order: 3
featured: true
role: "Graduation capstone · ongoing"
stack: "DINOv2 · RGB-D · ROS 2 Humble · Gazebo Classic 11"
excerpt: "A simulation-based UAV landing pipeline that scores candidate regions using semantic features and depth geometry."
---

The capstone addresses the gap between reaching a destination and finding a safe place to land. The current system combines DINOv2 features with depth-derived flatness, clearance, and proximity signals, then selects a candidate through a mission state machine.

The implementation includes ROS 2 nodes, Gazebo simulation, reactive depth-based obstacle handling, and a WPF monitoring direction for inspection. The project is explicitly simulation-based and ongoing; no real UAV flight or closed-loop robot deployment is claimed here.
