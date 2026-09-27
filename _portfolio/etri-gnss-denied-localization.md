---
title: "GNSS-Denied UAM Visual Localization"
collection: portfolio
permalink: /projects/gnss-denied-uam-localization/
order: 1
featured: true
role: "ETRI research engineering"
stack: "DINOv3 · FAISS · LightGlue · Jetson AGX Orin"
excerpt: "A two-stage aerial-image retrieval and matching pipeline for visual localization when GNSS is unavailable."
---

## Problem

Visual Place Recognition (VPR) for aerial views has to handle viewpoint, altitude, and heading changes while searching a large reference database. A pure descriptor search produced weak top-1 retrieval on the working evaluation setup.

## Engineering contribution

I designed a DINOv3 global-descriptor and FAISS retrieval pipeline, then narrowed the candidate set with altitude and heading metadata before LightGlue matching. I also investigated deployment behavior on Jetson AGX Orin and treated data-quality and latency issues as part of the system rather than as separate cleanup work.

The work is research and embedded deployment experience around an aerial-vision pipeline; it does not claim live aircraft operation.

## Evidence

The internal evaluation recorded Hit@1 improvement from 26.72% to 83.21% after metadata filtering. A related deployment measurement reached 0.74 seconds per image pair on Jetson AGX Orin.
