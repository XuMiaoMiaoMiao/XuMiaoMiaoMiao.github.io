---
title: Quadcopter Robust Control and Hardware-in-the-Loop Validation
date: 2023-06-01
summary: "Undergraduate thesis on robust quadcopter trajectory tracking, comparing cascaded PID and LADRC controllers through simulation and Pixhawk-AirSim hardware-in-the-loop validation."
tags:
  - Quadcopter Control
  - LADRC
  - PID
  - Hardware-in-the-loop
  - AirSim
links:
  - name: Thesis
    url: "https://github.com/XuMiaoMiaoMiao/Quadcopter-control-algorithm_Graduation_Project/blob/main/Undergraduate_Thesis.pdf"
---

**Undergraduate Thesis, 2022-2023.**

![AirSim hardware-in-the-loop validation with cascaded PID.](pid-hil.png)

![AirSim hardware-in-the-loop validation with cascaded LADRC.](featured.png)

I studied robust low-level control for quadcopter trajectory tracking under model uncertainty and external disturbances.

I built a MATLAB/Simulink quadcopter simulation platform and designed cascaded PID and cascaded LADRC controllers, where LADRC actively estimates and compensates for disturbances during flight.

I compared the controllers through hovering, disturbance-rejection, robustness, and Pixhawk-AirSim hardware-in-the-loop tests.

The results showed that LADRC achieved stronger disturbance rejection and more stable tracking than PID under uncertain flight conditions.
