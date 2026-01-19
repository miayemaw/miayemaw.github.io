---
layout: page
title: AI-based Multi-agent Mission Planning
description: Agency for Defense Development Civil-Military Research Program
img: assets/img/4.jpg
importance: 5
category: work
---

# AI-Driven Multi-Agent Mission Planning & Autonomous Obstacle Avoidance
**Ph.D. Research | Fully Funded by the Agency for Defense Development (ADD) Civil-Military Research Program**
**Duration:** 2019 - 2021  

### 01. Research Objective
**Problem Statement:** "How can we enable autonomous aerial vehicles to perform intelligent motion planning and real-time obstacle avoidance under dynamic, uncertain environments while ensuring kinematic and dynamic feasibility?"

This research addresses four core technical challenges:
* **Real-time Global Path Planning:** Fast and optimal path generation under dynamic environmental changes.
* **Local Planning:** Handling uncertainty and moving obstacles using Reinforcement Learning (RL)-based decision-making.
* **Trajectory Feasibility:** Ensuring planned paths respect UAV kinematic and dynamic constraints for stable control.
* **Modular Multi-Agent Integration:** Coordinating planning, avoidance, and control agents efficiently without latency bottlenecks.

**Overall System Architecture:**

![Overall System Architecture](assets/img/4.jpg)
*Figure 1: Modular Multi-Agent Framework integrating Path Planning, Obstacle Avoidance, and System Monitoring.*

---

### 02. Technical Novelty: iADA* & RL Integration

#### **Global Path Planning (iADA*)**
* Developed the **iADA*** algorithm, featuring minimum-cost calculation and optimized memory usage.
* Introduced a **"virtual wall"** feature to manage C-space obstacles effectively.

![iADA Flowchart](assets/img/4_2.jpg) ![iADA Demo](assets/img/4_3.gif)
*Left: iADA* Algorithm logic. Right: Real-time replanning performance.*

#### **Local Planning (DQN-based RL)**
* Integrated a **DQN-based local planner** for collision avoidance in dynamic environments.
* Combined perception with **UAV flight dynamics** (Translational/Rotational) for physically feasible trajectories.

![DQN Architecture](assets/img/4_4.jpg)
*Detailed DQN network architecture and UAV dynamic constraints.*

---

### 03. Performance & Results
* **Speed:** iADA* achieved a total planning time of **15.16ms**, significantly faster than D* Lite.
* **Reliability:** The iADA*-RL system reached a **94% success rate** in dynamic environments.

![Results Image](assets/img/4_5.gif) ![Results GIF](assets/img/4_6.gif)
*Simulation validation using AirSim and Unreal Engine 4.*

---

### 04. Future Extensions & Impact
* **MUM-T:** Building Collaboration Mission Planning for Manned-Unmanned Teaming.
* **UAM:** Extending frameworks for cooperative Urban Air Mobility operations.
* **Real-world Deployment:** Energy-aware planning for embedded UAV platforms.
