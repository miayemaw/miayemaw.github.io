---
layout: page
title: AI-based Multi-agent Mission Planning
description: Fully Funded Ph.D. Project (ADD Civil-Military Research)
img: assets/img/4.jpg
importance: 3
category: work
---

# AI-Driven Multi-Agent Mission Planning & Autonomous Obstacle Avoidance
**Ph.D. Research | Fully Funded by the Agency for Defense Development (ADD)**

### 01. Research Objective
**Problem Statement:** "How can we enable autonomous aerial vehicles to perform intelligent motion planning and real-time obstacle avoidance under dynamic, uncertain environments while ensuring kinematic and dynamic feasibility?"

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/4.jpg" title="Overall System Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1: Modular Multi-Agent Framework integrating Path Planning (PPRA), Obstacle Avoidance (ODA), and System Monitoring (SMA).
</div>

---

### 02. Technical Novelty: iADA* Algorithm

I developed the **iADA*** (Enhanced Anytime Path Planning) algorithm, featuring minimum-cost calculation and optimized memory usage compared to traditional D* Lite.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/4_2.jpg" title="iADA Algorithm Logic" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Internal logic of the iADA* algorithm, including the "virtual wall" feature for C-space obstacle management.
</div>

<div class="row justify-content-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/4_3.gif" title="iADA Real-time Performance" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Real-time replanning performance of iADA* in a dynamic maze environment.
</div>

---

### 03. Local Planning: DQN-based RL Integration

To handle moving obstacles, I integrated a **Deep Q-Network (DQN)** based local planner that respects strict UAV kinematic and dynamic constraints.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/4_4.jpg" title="DQN Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Detailed DQN network architecture and the 6-DOF flight dynamics model used for trajectory feasibility validation.
</div>

---

### 04. Performance & Outputs

The integrated **iADA*-RL** system was validated through 5,000 test cases, achieving a **94% success rate** and a planning speed of **15.16ms**.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/4_5.gif" title="Simulation Output Static" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/4_6.gif" title="Simulation Output Dynamic" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    High-fidelity simulation validation using AirSim and Unreal Engine 4 for multi-agent coordination.
</div>

---

### 05. Technical Stack
* **Algorithms:** iADA*, DQN (Reinforcement Learning), 6-DOF Dynamics.
* **Frameworks:** Keras, TensorFlow, OpenAI Gym, ROS, OctoMap.
* **Simulators:** AirSim (Microsoft), Unreal Engine 4 (UE4).