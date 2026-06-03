---
title: "COVER: Cross-Vehicle Transition Framework for Quadrotor Control"
date: 2025-01-01
summary: "Published air-ground cooperation framework for smooth UAV transfer between moving UGVs using non-inertial UGV body-frame control and stage-adaptive MPC."
tags:
  - UAV/UGV Cooperation
  - Model Predictive Control
  - Robotics
  - Non-inertial Frames
links:
  - name: Paper
    url: "https://link.springer.com/article/10.1007/s10514-025-10209-4"
  - name: Media
    url: "https://www.bilibili.com/video/BV1oBYrzVEzV/?spm_id_from=333.337.search-card.all.click&vd_source=d8b8395f653c5b027924f448228dcca5"
---

**Research Assistant, [FAST Lab](https://fast-fire.github.io/), Zhejiang University, 2023-2025.**

![Smooth cross-vehicle quadrotor transition between moving UGVs in air-ground cooperation.](featured.png)

I contributed to COVER, a published quadrotor-control framework for smooth cross-vehicle UAV transfer between moving UGVs.

The framework controls the UAV in UGV body frames modeled as non-inertial frames, eliminating dependence on a global world-frame trajectory.

It decomposes the maneuver into initial, transition, and final stages, generates dynamically feasible references through nonlinear programming, and uses a stage-adaptive MPC to suppress frame-switching instability and avoid indirect transition routes.

I assisted with real-world experiments, where we achieved the first smooth, short-distance, and accurate cross-vehicle transition demonstration in this system.
