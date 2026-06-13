---
title: Safe Reinforcement Learning for Bimanual Peg-in-Hole Manipulation
date: 2026-03-01
summary: "Isaac Sim benchmark for constrained bimanual peg-in-hole manipulation, comparing SAC and Lagrangian SAC with rollout-level safety-cost analysis."
tags:
  - Safe RL
  - Reinforcement Learning
  - Bi-manual Manipulation
  - Isaac Sim
  - Robotics
video:
  preview_url: /uploads/safe-rl-bimanual-demo.mp4
  preview_file: static/uploads/safe-rl-bimanual-demo.mp4
  detail_url: /uploads/safe-rl-bimanual-demo.mp4
  detail_file: static/uploads/safe-rl-bimanual-demo.mp4
slides: /uploads/cs-project-safe-rl-video-autoplay-loop.pptx
slides_file: static/uploads/cs-project-safe-rl-video-autoplay-loop.pptx
slides_embed: "https://view.officeapps.live.com/op/embed.aspx?src=https%3A%2F%2Fxumiaomiaomiao.github.io%2Fuploads%2Fcs-project-safe-rl-video-autoplay-loop.pptx"
links:
  - name: Code
    url: "https://github.com/XuMiaoMiaoMiao/Safe_RL_Peg_in_hole"
  - name: Report
    url: "/uploads/cs-project-report.pdf"
---

**Course Project, Lund University, 2026.**

{{< project-video >}}

{{< project-slides >}}

![Isaac Sim rollout for the bimanual peg-in-hole task.](featured.jpg)

![Rollout-level safety-cost curve comparing SAC and Lagrangian SAC.](safety-cost.png)

I built an Isaac Sim benchmark for bimanual peg-in-hole manipulation with two KUKA iiwa arms, where a 14-DoF joint-velocity policy coordinates the peg and hole.

I formulated the task as a constrained reinforcement learning problem by separating geometric task reward from safety cost, using peg-in-hole progress as reward and clearance violations as the cost signal.

I implemented SAC and Lagrangian SAC under the same environment, reward, cost, and evaluation protocol, with multi-seed training, deterministic evaluation, and rollout-level cost analysis.

In the current 15-seed Stage-1 harder-pose benchmark, Lagrangian SAC reduced episodic cost from **4.011 to 2.456** and cumulative sphere-proxy clearance-violation events from **2575.0 to 516.8**, while maintaining comparable task performance.
