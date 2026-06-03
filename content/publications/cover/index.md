---
title: 'COVER: cross-vehicle transition framework for quadrotor control in air-ground cooperation'
authors:
  - Qiuyu Ren
  - me
  - Mengke Zhang
  - Nanhe Chen
  - Mingwei Lai
  - Chao Xu
  - Fei Gao
  - Yanjun Cao
date: '2025-09-03T00:00:00Z'
publishDate: '2025-09-03T00:00:00Z'
publication_types: ['article-journal']
publication: 'Autonomous Robots, 49(3), 23'
publication_short: 'Autonomous Robots'
abstract: |
  This paper proposes COVER, a published quadrotor-control framework for smooth cross-vehicle UAV transfer between moving UGVs. The framework controls the UAV directly in UGV body frames modeled as non-inertial frames, reducing reliance on world-frame trajectory replanning and supporting accurate transitions between moving ground vehicles.
summary: 'Published cross-vehicle transition framework for quadrotor control in UAV/UGV air-ground cooperation.'
tags:
  - UAV Control
  - Air-Ground Cooperation
  - Model Predictive Control
  - Robotics
featured: true
hugoblox:
  ids:
    doi: 10.1007/s10514-025-10209-4
links:
  - type: doi
    url: https://doi.org/10.1007/s10514-025-10209-4
  - type: media
    url: "https://www.bilibili.com/video/BV1oBYrzVEzV/?spm_id_from=333.337.search-card.all.click&vd_source=d8b8395f653c5b027924f448228dcca5"
image:
  caption: ''
  focal_point: ''
  preview_only: false
projects:
  - air-ground-cooperation
slides: ""
video:
  embed_url: "https://player.bilibili.com/player.html?bvid=BV1oBYrzVEzV&page=1&autoplay=0&high_quality=1"
---

This work introduces a transition framework for quadrotor operations across moving UGVs in air-ground cooperation.

The framework controls the UAV in UGV body frames modeled as non-inertial frames, eliminating dependence on a global world-frame trajectory.

It decomposes the maneuver into initial, transition, and final stages, generates dynamically feasible references through nonlinear programming, and uses a stage-adaptive MPC to suppress frame-switching instability and avoid indirect transition routes.

The real-world system demonstrates smooth, short-distance, and accurate cross-vehicle transition between moving UGVs.
