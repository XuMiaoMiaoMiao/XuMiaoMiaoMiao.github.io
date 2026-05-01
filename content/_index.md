---
title: ''
summary: ''
date: 2026-05-01
type: landing

sections:
  - block: resume-biography-3
    content:
      username: me
      text: |
        I study reliable autonomy for aerial and cooperative robotic systems.
        My recent work focuses on model-based and learning-based control for quadrotors, especially air-ground cooperative tasks and dynamic-platform landing.
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: About
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: lg
      avatar:
        size: large
        shape: circle

  - block: markdown
    id: research
    content:
      title: Research Direction
      subtitle: Robotics, control, and autonomous aerial systems
      text: |
        My research aims to build accurate, robust, and deployable control systems for autonomous robots.
        I am particularly interested in combining model predictive control, adaptive control, and learning-based perception/control for UAVs and heterogeneous robot teams.

        Current themes include:
        - **Air-ground cooperative robotics:** relative-state modelling and control for UAV/UGV interaction without relying on global state estimation.
        - **Dynamic-platform landing:** robust quadrotor landing using robocentric modelling, relative visual feedback, and adaptive MPC.
        - **Learning-based control:** integrating data-driven modules with interpretable model-based controllers for agile robotic tasks.
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Featured Publication
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: citation

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: Selected research and engineering projects related to robotics, aerial systems, and control.
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 3
      fill_image: false
      show_date: false
      show_read_time: false
      show_read_more: false
---
