---
layout: page
title: AI Digital Twin for Smart Urban Air Mobility
description: National Research Foundation of Korea (NRF) project
img: assets/img/ODT.gif
importance: 1
category: work
---

**Duration:** 2020 - 2029  
**Funding:** National Research Foundation of Korea (NRF) funded by the Ministry of Education  
**Role:** Project Manager

# Operational Digital Twin (ODT) Framework for UAM
**Advanced Research in Predictive Simulation, AI Perception, and Decision Support**

### 01. Project Vision
**Problem Statement:** "How can we develop a high-fidelity, AI-enabled digital twin platform that can replicate, predict, and support decision-making for complex UAM operations in urban cities?"

This research bridges the gap between digital simulation and real-world operations to ensure safety assurance and future digital certification for eVTOL and UAV platforms.

---

### 02. Overall Architecture & System Design

To support complex UAM operations, the framework is built on a modular, high-interoperability architecture.

#### **A. DTAM Operational Flow**
This high-level overview illustrates the five pillars of the **Digital Twin for Air Mobility (DTAM)**: the ODT Core, Mission Planning, Situation Awareness, AI Plugins, and Application Plugins.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_1.png" title="DTAM Operational Flow" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Digital Twin for Air Mobility (DTAM) operational pillars: ODT Core, Mission Setup, Situation Awareness, AI Plugins, and Application Plugins.
</div>


#### **B. ODT Modular Core Modules**
This schematic details the internal communication between Sensing, Flight Authoring, and Vehicle Core modules. It highlights the use of **RPC/UDP APIs** to connect the simulation core with third-party application modules like Traffic Management and AI Training.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_2.png" title="ODT Modular Core Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Detailed modular core architecture showing internal communication between Sensing, Flight Authoring, and Vehicle modules via RPC/UDP APIs.
</div>
---

### 03. Core Technologies & Innovation

#### **[1] High-Fidelity UAM Simulation**
* **Realistic Environments:** Developed urban models featuring vertiports, traffic, and high-accuracy vehicle dynamics.
* **4D Trajectory:** Implemented real-time trajectory generation and airspace prediction.
* **Flight Control:** Integrated MAVLINK interfaces with **6-DOF Equations of Motion (EOM)** for hardware-in-the-loop (HIL) validation.

#### **[2] AI Perception & Decision Support**
* **Perception:** Integrated **R-YOLO** for real-time dynamic obstacle and bird-strike detection.
* **Decision Logic:** Utilized **AHP (Analytic Hierarchy Process)** and adaptive **ACAS Xu** for multi-agent coordination and risk scoring.
* **Temporal Processing:** Leveraged CNNs and temporal models to provide live advisories to operators.

#### **[3] Optimization & Scalability**
* Developed multi-objective trajectory and scheduling optimization.
* Built a dashboard for real-time what-if scenario analysis and operational playback.

---

### 04. Performance & Validation
Unlike conventional digital twins that focus on offline post-analysis, this platform operates at a **~1 Hz refresh rate**, enabling live operational visualization.

| Feature | Conventional Digital Twins | ODT (This Work) |
| :--- | :--- | :--- |
| **Modularity** | Limited/Static | Fully modular 3-layer (Sim – AI – Vis) |
| **AI Integration** | Minimal | Precision Decision AI (R-YOLO, ACAS Xu, RL) |
| **Real-time Capability** | Offline post-analysis | Live simulation & predictive trajectories (~1Hz) |
| **Interoperability** | Usually standalone | Connects via APIs to planners and external models |

---

### 05. Interactive Demo
Experience the platform firsthand. You can log in to the web-based demo to test vertiport management, trajectory planning, and real-time safety analysis.

<div class="row justify-content-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_3.gif" title="ODT System Demo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Real-time operational dashboard demonstration showing vertiport management, 4D trajectory planning, and safety analysis.
</div>


**[🚀 Access Live UAM Demo](http://203.252.161.46:2025/)**
*(Note: Use your credentials to explore the dashboard and scenario playback features.)*

---

### 06. Technical Stack
* **Simulation:** UAMSim, Unreal Engine 4, PX4/MAVLINK/CustomControl.
* **AI/ML:** R-YOLO, CNNs, Reinforcement Learning (DQN, PPO), Keras/TensorFlow.
* **Communication:** RPC / UDP / TCP / API, MAVLINK.
* **Analytics:** AHP-based decision modules, Multi-objective optimization.
* **Available Plugins:** Mission Plans (Upload, Customize), Situation Awareness, Traffic Management