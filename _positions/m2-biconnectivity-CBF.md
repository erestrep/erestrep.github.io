---
layout: page
title: Resilient Coordination of Multi-robot Systems: Enabling Long-Term Autonomy
description: Open research internship position (stage M2)
img: assets/img/connect.png
importance: 2
category: Master thesis
giscus_comments: true
---

**Short abstract:** This Master's Thesis will focus on proposing a **distributed Control Barrier Function (CBF)** strategy to enable persistent autonomy in **Open Multi-Robot Systems**. The framework guarantees safety and biconnectivity during dynamic agent addition and removal, facilitating long-term missions that outlast individual battery lives.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/connect.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Snapshot of an simulation of drone coordination using the generalized connectivity model in [1].
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Esteban Restrepo](https://erestrep.github.io/), [Nicola De Carli](https://www.kth.se/profile/ndc)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [ndc@kth.se](mailto:ndc@kth.se)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-res-coord/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description and motivation:** Most multi-robot research assumes a "closed" system: a fixed team of agents starts and finishes a task together. However, real-world applications—such as continuous environmental monitoring, perimeter surveillance, or smart logistics—require **Long-Term Autonomy**. In these missions, the task duration far exceeds the battery life of any single robot. To bridge this gap, we must move toward **Open Multi-Robot Systems**. These are dynamic ecosystems where the population is fluid: agents must leave to recharge or undergo maintenance, while new agents enter to replace them or scale up the operation. The "swapping" of robots must be seamless. The departure of an agent (or its sudden failure) creates a risk of fracturing the communication network or violating coverage constraints. Conversely, the addition of a new agent introduces integration challenges in collision avoidance and formation merging.

This thesis proposes a robust, distributed control framework that treats the robot population as a time-varying variable. It builds upon two key pillars:

1. Generalized Biconnectivity [1-2]: A graph-theoretic framework ensuring the network remains structurally intact (robust to single-point failures) even as nodes are added or removed. It encodes operational constraints (sensing, communication) into the graph weights.
1. Control Barrier Functions (CBFs) [3]: A safety-critical control method that strictly enforces constraints. We will use CBFs to create a "safe harbor" for agents entering or leaving the system, ensuring that topological changes never trigger collisions or disconnect the fleet.


**General Objectives:** The goal is to develop a distributed strategy for resilient coordination in Open Multi-Robot Systems, enabling persistent operation despite constant changes in the team composition.

The student will:

* Formulate a **distributed Control Barrier Function (CBF)** controller that adapts to a time-varying number of agents, guaranteeing safety during "Plug-and-Play" maneuvers.

* Develop a protocol based on **Generalized Biconnectivity** that allows the swarm to autonomously reconfigure its topology when agents join or leave, preventing network fragmentation.

* Design a **"persistent mission"** scenario (e.g., area coverage or patrolling) where robots cycle between active duty and a charging station.

* Validate the approach through **extensive simulation and hardware experiments** using a heterogeneous team (ground robots and mini-drones), demonstrating that the mission continues uninterrupted while the hardware is swapped out.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the experimental setup in the team.

2. Take over the existing works and work on the CBF-based distributed and resilient coordination strategy for a multi-robot system.

3. Implement and validate in simulation the proposed algorithms.

4. Validate experimentally the scenario on a team of mobile robots.

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation and interest in the topic

* Good knowledge in control theory and robot modeling

* Basic knowledge of control and analysis of multi-agent systems

* Previous experience with Python/C++ and ROS2

* Scientific curiosity

<br>
<hr>
<br>

<h3 class="subsection-title">Conditions</h3>
<br>

Expected duration of the internship: **5-6 months**

The work will be carried in English at the Centre Inria de l’Université de Rennes research center in Rennes, France.

Financial support offered to the student: gratification de 4,35 € / h

<br>
<h3 class="subsection-title">How to apply</h3>
<br>

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-res-coord/).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Nicola De Carli

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Restrepo, E., & Robuffo Giordano, P. (2024, December). A Distributed Strategy for Generalized Biconnectivity Maintenance in Open Multi-robot Systems. In 2024 IEEE 63rd Conference on Decision and Control (CDC) (pp. 3043-3050). IEEE.

2. Restrepo, E., & Robuffo Giordano, P. (2023). Distributed biconnecitvity achievement and preservation in multi-agent systems. IEEE Control Systems Letters, 7, 3289-3294.

3. De Carli, N., Salaris, P., & Giordano, P. R. (2024, May). Distributed control barrier functions for global connectivity maintenance. In 2024 IEEE International Conference on Robotics and Automation (ICRA) (pp. 12048-12054). IEEE.

4. P. Robuffo Giordano, Q. Delamare, A. Franchi. Trajectory Generation for Minimum Closed-Loop State Sensitivity. In IEEE Int. Conf. on Robotics and Automation, ICRA’18, Pages 286-293, Brisbane, Australia, May 2018

5. Ames, A. D., Coogan, S., Egerstedt, M., Notomista, G., Sreenath, K., & Tabuada, P. (2019, June). Control barrier functions: Theory and applications. In 2019 18th European control conference (ECC) (pp. 3420-3431). IEEE.

