---
title: "Foundation Models on Edge Hardware"
collection: portfolio
permalink: /projects/edge-deployment/
order: 2
featured: true
role: "Edge inference and systems optimization"
stack: "ONNX · Jetson AGX Orin · Raspberry Pi 5 · Hailo-10H"
excerpt: "Turning vision research pipelines into measurable inference systems on constrained hardware."
---

I have worked across server and embedded targets rather than treating deployment as an afterthought. This includes ONNX conversion and runtime measurement on Jetson AGX Orin, and an end-to-end visual localization deployment on Raspberry Pi 5 with a Hailo-10H NPU.

One optimization investigation traced a 5.6-second query path to repeated reference-database loading; retaining the database reduced the measured latency to 325 ms. The result is a practical systems lesson: profiling the pipeline boundary can matter as much as changing the model.

These are software and hardware-in-the-loop deployment experiences. They should not be read as evidence of production autonomy or real-flight operation.
